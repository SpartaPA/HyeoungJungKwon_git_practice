# udev rule key table

| Key | Meaning |
|---|---|
| `SUBSYSTEM` | Kernel subsystem condition |
| `KERNEL` | Kernel device name condition |
| `ATTR{}` | Current device sysfs attribute |
| `SYMLINK+=` | Add a stable `/dev` alias |
| `MODE` | Device permission mode |
| `GROUP` | Device group ownership |
