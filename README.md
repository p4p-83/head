# `gantry`

> [!NOTE]
> Refer to [`p4p.jamesnzl.xyz/learn`](https://p4p.jamesnzl.xyz/learn) for full details.

This repository contains the low-level machine control for our head mechanism, pneumatics, and vacuum nozzle for our pick-and-place machine.

## Usage

Firstly, clone this repository.

This repository is structured as a [PlatformIO](https://platformio.org/) project.

```sh
git submodule update --init
code .
```

## Interfaces

### USB

- A USB serial port at `115200` baud is used to exchange data between this firmware and the [`p4p-83/controller`](https://github.com/p4p-83/controller).

#### Protocol Buffers

- [Protocol buffers](https://protobuf.dev/overview/) are used for data exchange.
- See [`p4p-83/protobufs`](https://github.com/p4p-83/protobufs) for the `.proto` definition(s).
