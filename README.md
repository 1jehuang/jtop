# jtop - A Process-Focused System Monitor

Forked from [btop](https://github.com/aristocratos/btop) with a focus on **process visibility**.

## What's Different?

**jtop's main feature:** Split process view showing **top CPU users** and **top memory users** side by side!

```
┌─────────────────────┬─────────────────────┐
│  Top CPU Consumers  │ Top Memory Consumers│
├─────────────────────┼─────────────────────┤
│ firefox    45.2%    │ chrome    2.3GB     │
│ code       23.1%    │ firefox   1.8GB     │
│ chrome     12.5%    │ code      1.2GB     │
│ ...                 │ ...                 │
└─────────────────────┴─────────────────────┘
```

## Features

- ✅ **Split process view** - See top CPU and top memory users simultaneously
- ✅ Beautiful, customizable themes (inherited from btop)
- ✅ Interactive process management (kill, filter, search)
- ✅ CPU, memory, network, and disk monitoring
- ✅ GPU support (NVIDIA, AMD, Intel)
- ✅ Tree view for processes
- ✅ Mouse support

## Installation

### From Source

```bash
git clone https://github.com/1jehuang/jtop.git
cd jtop
make
sudo make install
```

### Requirements

- C++23 compatible compiler (GCC 13+, Clang 16+)
- CMake 3.25+
- Linux, macOS, FreeBSD, NetBSD, or OpenBSD

## Keybindings

| Key | Action |
|-----|--------|
| `1` | Toggle split process view |
| `y` | Cycle process sort mode |
| `f` | Filter processes |
| `k` | Kill selected process |
| `e` | Toggle tree view |
| `?` | Help menu |
| `q` | Quit |

## Credits

- Original project: [btop](https://github.com/aristocratos/btop) by Aristocratos
- Fork maintained by [1jehuang](https://github.com/1jehuang)

## License

Apache License 2.0 (same as btop)
