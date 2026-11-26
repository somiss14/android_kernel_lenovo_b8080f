# android_kernel_lenovo_b8080f

Kernel UAPI source snapshot for **Lenovo Yoga Tablet 10 HD+ (B8080-F)** — Lenovo b8080f 3.4.0 kernel source, single-commit tree (the original Lenovo/upstream history carries file modes GitHub refuses to accept).

Used only for `make headers_install`: the device tree builds with Lenovo's **prebuilt** stock kernel (see `device/lenovo/b8080f`), and the Qualcomm HALs compile against the headers exported from this tree.

Key local change vs the base tree (`android_kernel_motorola_msm8226` @ 22bc4ed7f41, lineage-14.1): `include/linux/msm_mdp.h` — `pipe_type` moved to the end of `struct mdp_overlay` to match the stock Lenovo kernel ABI.

The branch `b8080f-14.1-full` in the port workspace preserves the full original history including the pipe_type fix as a normal commit, for anyone with a git host that accepts it.
