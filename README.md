# PartyPlayKit

Shared local-party infrastructure for [Empires](https://github.com/utopastac/empires-ios) and [Doodleoop](https://github.com/utopastac/doodleoop-ios).

## Contents

- **MultipeerTransport** — Bonjour advertise/browse + reliable `Data` / `Codable` send; apps choose `serviceType`
- **DeviceIdentity** — persisted phone UUID (`deviceId`)
- **SeatPlayer / SeatHandoff** — multi-seat-on-one-phone primitives (UI stays in each app)

## Not included (on purpose)

Game engines, wire message enums, themes, and screens stay app-specific.

## Consume

Clone next to each app and depend via local path:

```yaml
# XcodeGen
packages:
  PartyPlayKit:
    path: ../party-play-kit
```

```
code/
  party-play-kit/
  empires-ios/
  doodleoop-ios/
```
