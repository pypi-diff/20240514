# Comparing `tmp/riscemu-2.2.5.tar.gz` & `tmp/riscemu-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riscemu-2.2.5.tar", max compression
+gzip compressed data, was "riscemu-2.2.6.tar", max compression
```

## Comparing `riscemu-2.2.5.tar` & `riscemu-2.2.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1074 2023-10-12 15:12:27.576277 riscemu-2.2.5/LICENSE
--rw-r--r--   0        0        0     4903 2023-10-12 15:12:27.576277 riscemu-2.2.5/README.md
--rw-r--r--   0        0        0      950 2023-10-12 15:12:27.580277 riscemu-2.2.5/pyproject.toml
--rw-r--r--   0        0        0      829 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/IO/IOModule.py
--rw-r--r--   0        0        0     1559 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/IO/TextIO.py
--rw-r--r--   0        0        0        0 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/IO/__init__.py
--rw-r--r--   0        0        0      455 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/__init__.py
--rw-r--r--   0        0        0      569 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/__main__.py
--rw-r--r--   0        0        0     9089 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/assembler.py
--rw-r--r--   0        0        0      559 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/colors.py
--rw-r--r--   0        0        0      730 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/config.py
--rw-r--r--   0        0        0     2314 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/__init__.py
--rw-r--r--   0        0        0     1717 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/binary_data_memory_section.py
--rw-r--r--   0        0        0     4508 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/cpu.py
--rw-r--r--   0        0        0     7119 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/csr.py
--rw-r--r--   0        0        0     1679 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/csr_constants.py
--rw-r--r--   0        0        0     4810 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/exceptions.py
--rw-r--r--   0        0        0      262 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/flags.py
--rw-r--r--   0        0        0     5741 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/float.py
--rw-r--r--   0        0        0     1835 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/instruction.py
--rw-r--r--   0        0        0     1888 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/instruction_context.py
--rw-r--r--   0        0        0     1496 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/instruction_memory_section.py
--rw-r--r--   0        0        0     8590 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/int32.py
--rw-r--r--   0        0        0     5535 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/memory_section.py
--rw-r--r--   0        0        0    12783 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/mmu.py
--rw-r--r--   0        0        0      509 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/platform.py
--rw-r--r--   0        0        0      110 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/privmodes.py
--rw-r--r--   0        0        0     4143 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/program.py
--rw-r--r--   0        0        0     2149 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/program_loader.py
--rw-r--r--   0        0        0     6714 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/registers.py
--rw-r--r--   0        0        0      683 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/rtclock.py
--rw-r--r--   0        0        0     1646 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/simple_instruction.py
--rw-r--r--   0        0        0     3107 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/traps.py
--rw-r--r--   0        0        0     3959 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/core/usermode_cpu.py
--rw-r--r--   0        0        0     2240 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/debug.py
--rw-r--r--   0        0        0      133 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/decoder/__init__.py
--rw-r--r--   0        0        0      589 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/decoder/__main__.py
--rw-r--r--   0        0        0     2648 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/decoder/decoder.py
--rw-r--r--   0        0        0     2283 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/decoder/formats.py
--rw-r--r--   0        0        0     1349 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/decoder/formatter.py
--rw-r--r--   0        0        0     1842 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/decoder/instruction_table.py
--rw-r--r--   0        0        0      341 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/decoder/regs.py
--rw-r--r--   0        0        0     3337 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/helpers.py
--rw-r--r--   0        0        0     3185 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/instructions/RV32A.py
--rw-r--r--   0        0        0      575 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/instructions/RV32D.py
--rw-r--r--   0        0        0     4926 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/instructions/RV32F.py
--rw-r--r--   0        0        0     9573 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/instructions/RV32I.py
--rw-r--r--   0        0        0     1324 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/instructions/RV32M.py
--rw-r--r--   0        0        0     1913 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/instructions/RV_Debug.py
--rw-r--r--   0        0        0     3145 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/instructions/Zicsr.py
--rw-r--r--   0        0        0      658 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/instructions/__init__.py
--rw-r--r--   0        0        0    11666 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/instructions/float_base.py
--rw-r--r--   0        0        0     4330 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/instructions/instruction_set.py
--rw-r--r--   0        0        0     1002 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/interactive.py
--rw-r--r--   0        0        0      670 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/libc/README.md
--rw-r--r--   0        0        0      345 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/libc/crt0.s
--rw-r--r--   0        0        0     4518 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/libc/stdlib.s
--rw-r--r--   0        0        0     4751 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/libc/string.s
--rw-r--r--   0        0        0     4987 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/parser.py
--rw-r--r--   0        0        0     4614 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/priv/CSR.py
--rw-r--r--   0        0        0     4143 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/priv/ElfLoader.py
--rw-r--r--   0        0        0     2854 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/priv/ImageLoader.py
--rw-r--r--   0        0        0     8536 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/priv/PrivCPU.py
--rw-r--r--   0        0        0     1685 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/priv/PrivMMU.py
--rw-r--r--   0        0        0     6117 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/priv/PrivRV32I.py
--rw-r--r--   0        0        0      455 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/priv/__init__.py
--rw-r--r--   0        0        0     1705 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/priv/__main__.py
--rw-r--r--   0        0        0     5212 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/priv/types.py
--rw-r--r--   0        0        0        0 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/py.typed
--rw-r--r--   0        0        0    12018 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/riscemu_main.py
--rw-r--r--   0        0        0     8423 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/syscall.py
--rw-r--r--   0        0        0     3281 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/tokenizer.py
--rwxr-xr-x   0        0        0       44 2023-10-12 15:12:27.580277 riscemu-2.2.5/riscemu/tools/riscemu
--rw-r--r--   0        0        0     5767 1970-01-01 00:00:00.000000 riscemu-2.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-14 11:45:59.700418 riscemu-2.2.6/LICENSE
+-rw-r--r--   0        0        0     5381 2024-05-14 11:45:59.700418 riscemu-2.2.6/README.md
+-rw-r--r--   0        0        0      950 2024-05-14 11:45:59.704418 riscemu-2.2.6/pyproject.toml
+-rw-r--r--   0        0        0      829 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/IO/IOModule.py
+-rw-r--r--   0        0        0     1559 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/IO/TextIO.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/IO/__init__.py
+-rw-r--r--   0        0        0      455 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/__init__.py
+-rw-r--r--   0        0        0      569 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/__main__.py
+-rw-r--r--   0        0        0     9089 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/assembler.py
+-rw-r--r--   0        0        0      559 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/colors.py
+-rw-r--r--   0        0        0      730 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/config.py
+-rw-r--r--   0        0        0     2314 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/__init__.py
+-rw-r--r--   0        0        0     1717 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/binary_data_memory_section.py
+-rw-r--r--   0        0        0     4508 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/cpu.py
+-rw-r--r--   0        0        0     7119 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/csr.py
+-rw-r--r--   0        0        0     1679 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/csr_constants.py
+-rw-r--r--   0        0        0     4810 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/exceptions.py
+-rw-r--r--   0        0        0      262 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/flags.py
+-rw-r--r--   0        0        0     5963 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/float.py
+-rw-r--r--   0        0        0     1835 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/instruction.py
+-rw-r--r--   0        0        0     1888 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/instruction_context.py
+-rw-r--r--   0        0        0     1496 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/instruction_memory_section.py
+-rw-r--r--   0        0        0     9469 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/int32.py
+-rw-r--r--   0        0        0     5535 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/memory_section.py
+-rw-r--r--   0        0        0    12783 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/mmu.py
+-rw-r--r--   0        0        0      509 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/platform.py
+-rw-r--r--   0        0        0      110 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/privmodes.py
+-rw-r--r--   0        0        0     4143 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/program.py
+-rw-r--r--   0        0        0     2149 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/program_loader.py
+-rw-r--r--   0        0        0     6712 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/registers.py
+-rw-r--r--   0        0        0      683 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/rtclock.py
+-rw-r--r--   0        0        0     1646 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/simple_instruction.py
+-rw-r--r--   0        0        0     3107 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/traps.py
+-rw-r--r--   0        0        0     3959 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/core/usermode_cpu.py
+-rw-r--r--   0        0        0     2240 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/debug.py
+-rw-r--r--   0        0        0      133 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/decoder/__init__.py
+-rw-r--r--   0        0        0      589 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/decoder/__main__.py
+-rw-r--r--   0        0        0     2648 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/decoder/decoder.py
+-rw-r--r--   0        0        0     2283 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/decoder/formats.py
+-rw-r--r--   0        0        0     1349 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/decoder/formatter.py
+-rw-r--r--   0        0        0     1842 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/decoder/instruction_table.py
+-rw-r--r--   0        0        0      341 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/decoder/regs.py
+-rw-r--r--   0        0        0     3337 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/helpers.py
+-rw-r--r--   0        0        0     3185 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/instructions/RV32A.py
+-rw-r--r--   0        0        0     3588 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/instructions/RV32D.py
+-rw-r--r--   0        0        0     4931 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/instructions/RV32F.py
+-rw-r--r--   0        0        0     9573 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/instructions/RV32I.py
+-rw-r--r--   0        0        0     1500 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/instructions/RV32M.py
+-rw-r--r--   0        0        0     1913 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/instructions/RV_Debug.py
+-rw-r--r--   0        0        0     3145 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/instructions/Zicsr.py
+-rw-r--r--   0        0        0      658 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/instructions/__init__.py
+-rw-r--r--   0        0        0    11666 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/instructions/float_base.py
+-rw-r--r--   0        0        0     4330 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/instructions/instruction_set.py
+-rw-r--r--   0        0        0     1002 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/interactive.py
+-rw-r--r--   0        0        0      670 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/libc/README.md
+-rw-r--r--   0        0        0      345 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/libc/crt0.s
+-rw-r--r--   0        0        0     4518 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/libc/stdlib.s
+-rw-r--r--   0        0        0     4751 2024-05-14 11:45:59.704418 riscemu-2.2.6/riscemu/libc/string.s
+-rw-r--r--   0        0        0     7011 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/parser.py
+-rw-r--r--   0        0        0     4614 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/priv/CSR.py
+-rw-r--r--   0        0        0     4143 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/priv/ElfLoader.py
+-rw-r--r--   0        0        0     2854 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/priv/ImageLoader.py
+-rw-r--r--   0        0        0     8536 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/priv/PrivCPU.py
+-rw-r--r--   0        0        0     1685 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/priv/PrivMMU.py
+-rw-r--r--   0        0        0     6117 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/priv/PrivRV32I.py
+-rw-r--r--   0        0        0      455 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/priv/__init__.py
+-rw-r--r--   0        0        0     1705 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/priv/__main__.py
+-rw-r--r--   0        0        0     5212 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/priv/types.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/py.typed
+-rw-r--r--   0        0        0    12018 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/riscemu_main.py
+-rw-r--r--   0        0        0     8423 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/syscall.py
+-rw-r--r--   0        0        0     3281 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/tokenizer.py
+-rwxr-xr-x   0        0        0       44 2024-05-14 11:45:59.708418 riscemu-2.2.6/riscemu/tools/riscemu
+-rw-r--r--   0        0        0     6296 1970-01-01 00:00:00.000000 riscemu-2.2.6/PKG-INFO
```

### Comparing `riscemu-2.2.5/LICENSE` & `riscemu-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/README.md` & `riscemu-2.2.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -98,7 +98,23 @@
   * RISC-V reference card: https://www.cl.cam.ac.uk/teaching/1617/ECAD+Arch/files/docs/RISCVGreenCardv8-20151013.pdf
 
 ## TODO:
  * Correctly handle 12 and 20 bit immediate (currently not limited to bits at all)
  * Add a cycle limit to the options and CPU to catch infinite loops
  * Move away from `print` and use `logging.logger` instead
  * Writer proper tests
+
+
+## How To Release:
+
+Create a new commit that:
+1. Changes the "Upcoming" heading to the new versions number
+2. Increments the version in the pyproject.toml to the next version
+
+Commit this, and tag it with `v<version>`. Push the commit and the tag:
+```bash
+git push
+git push origin "v<version>"
+```
+
+On GitHub, [draft a new release](https://github.com/AntonLydike/riscemu/releases/new), and
+then approve the workflow run [here](https://github.com/AntonLydike/riscemu/actions).
```

### Comparing `riscemu-2.2.5/pyproject.toml` & `riscemu-2.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "riscemu"
-version = "2.2.5"
+version = "2.2.6"
 description = "A basic RISC-V emulator"
 authors = ["Anton Lydike <me@antonlydike.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/antonlydike/riscemu"
 repository = "https://github.com/antonlydike/riscemu"
 keywords = ["RISC-V"]
```

### Comparing `riscemu-2.2.5/riscemu/IO/IOModule.py` & `riscemu-2.2.6/riscemu/IO/IOModule.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/IO/TextIO.py` & `riscemu-2.2.6/riscemu/IO/TextIO.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/__main__.py` & `riscemu-2.2.6/riscemu/__main__.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/assembler.py` & `riscemu-2.2.6/riscemu/assembler.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/colors.py` & `riscemu-2.2.6/riscemu/colors.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/config.py` & `riscemu-2.2.6/riscemu/config.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/__init__.py` & `riscemu-2.2.6/riscemu/core/__init__.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/binary_data_memory_section.py` & `riscemu-2.2.6/riscemu/core/binary_data_memory_section.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/cpu.py` & `riscemu-2.2.6/riscemu/core/cpu.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/csr.py` & `riscemu-2.2.6/riscemu/core/csr.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/csr_constants.py` & `riscemu-2.2.6/riscemu/core/csr_constants.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/exceptions.py` & `riscemu-2.2.6/riscemu/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/float.py` & `riscemu-2.2.6/riscemu/core/float.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import struct
+import warnings
 from ctypes import c_float, c_double
 from typing import Union, Any, ClassVar, Type
 from abc import ABC
 
 bytes_t = bytes
 
 
@@ -126,17 +127,14 @@
         if isinstance(other, BaseFloat):
             other = other.value
         return self.value >= other
 
     def __bool__(self):
         return bool(self.value)
 
-    def __int__(self):
-        return int(self.value)
-
     def __float__(self):
         return self.value
 
     def __pow__(self, power, modulo=None):
         if modulo is not None:
             raise ValueError("Float32 pow with modulo unsupported")
         return self.__class__(self.value**power)
@@ -188,14 +186,21 @@
     def __format__(self, spec: str):
         if spec[-2:] == "32":
             return Float32.bitcast(self).__format__(spec[:-2])
         if spec[-2:] == "64":
             return Float64.bitcast(self).__format__(spec[:-2])
         return format(self.value, spec)
 
+    def __int__(self):
+        warnings.warn(
+            "Float32.__int__ is deprecated due its inability to handle infities and NaNs correctly! Use {Int32,UInt32).from_float instead!",
+            DeprecationWarning,
+        )
+        return int(self.value)
+
 
 class Float32(BaseFloat):
     _type = c_float
     _struct_fmt_str = "f"
 
 
 class Float64(BaseFloat):
```

### Comparing `riscemu-2.2.5/riscemu/core/instruction.py` & `riscemu-2.2.6/riscemu/core/instruction.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/instruction_context.py` & `riscemu-2.2.6/riscemu/core/instruction_context.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/instruction_memory_section.py` & `riscemu-2.2.6/riscemu/core/instruction_memory_section.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/int32.py` & `riscemu-2.2.6/riscemu/core/int32.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Any, Union
+import math
+
+from typing import Any, Union, ClassVar
 from ctypes import c_int32, c_uint32
 
 
 class Int32:
     """
     This class implements 32bit signed integers (see :class:`UInt32` for unsigned integers)
 
@@ -11,14 +13,17 @@
     You can use it just like you would any other integer, just be careful when passing it
     to functions which actually expect an integer and not an Int32.
     """
 
     _type = c_int32
     __slots__ = ("_val",)
 
+    MIN_VALUE: ClassVar[int] = -(2**31)
+    MAX_VALUE: ClassVar[int] = 2**31 - 1
+
     def __init__(
         self, val: Union[int, c_int32, c_uint32, "Int32", bytes, bytearray, bool] = 0
     ):
         if isinstance(val, (c_uint32, c_int32, Int32)):
             self._val = self.__class__._type(val.value)
         elif isinstance(val, (int, bool)):
             self._val = self.__class__._type(val)
@@ -201,17 +206,15 @@
         return bytearray(self.unsigned_value.to_bytes(4, "little"))[0:bytes]
 
     def signed(self) -> "Int32":
         """
         Convert to a signed representation. See :class:Int32
         :return:
         """
-        if self.__class__ == Int32:
-            return self
-        return Int32(self)
+        return self
 
     @property
     def unsigned_value(self):
         """
         Return the value interpreted as an unsigned integer
         :return:
         """
@@ -251,22 +254,43 @@
         sign = data >> (bits - 1)
         if sign > 1:
             print("overflow in Int32.sext!")
         if sign:
             data = (data & (2 ** (bits - 1) - 1)) - 2 ** (bits - 1)
         return cls(data)
 
+    @classmethod
+    def from_float(cls, number: float) -> "Int32":
+        """
+        Convert a floating point number to an instance of Int32, handling overflows and NaN according to RISC-V spec.
+
+        - Valid values and infinities are clamped between MIN_VALUE and MAX_VALUE
+        - NaN is treated as -inf
+        """
+        if math.isnan(number):
+            number = cls.MIN_VALUE
+        elif number > cls.MAX_VALUE:
+            number = cls.MAX_VALUE
+        elif number < cls.MIN_VALUE:
+            number = cls.MIN_VALUE
+        else:
+            number = int(number)
+        return cls(number)
+
 
 class UInt32(Int32):
     """
     An unsigned version of :class:Int32.
     """
 
     _type = c_uint32
 
+    MIN_VALUE: ClassVar[int] = 0
+    MAX_VALUE: ClassVar[int] = 2**32 - 1
+
     def unsigned(self) -> "UInt32":
         """
         Return a new instance representing the same bytes, but signed
         :return:
         """
         return self
 
@@ -280,7 +304,11 @@
 
         :param amount: Number of positions to shift
         :return: A new Int32 object representing the shifted value (keeps the signed-ness of the source)
         """
         if isinstance(amount, Int32):
             amount = amount.value
         return UInt32(self.value >> amount)
+
+    def signed(self) -> "Int32":
+        # Overflow is handled natively by the underlying c_uint32 to c_int32 conversion!
+        return Int32(self._val)
```

### Comparing `riscemu-2.2.5/riscemu/core/memory_section.py` & `riscemu-2.2.6/riscemu/core/memory_section.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/mmu.py` & `riscemu-2.2.6/riscemu/core/mmu.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/program.py` & `riscemu-2.2.6/riscemu/core/program.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/program_loader.py` & `riscemu-2.2.6/riscemu/core/program_loader.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/registers.py` & `riscemu-2.2.6/riscemu/core/registers.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             reg = "s1"
         if mark_set:
             self.last_set = reg
 
         if not self.infinite_regs and reg not in self.valid_regs:
             raise RuntimeError("Invalid register: {}".format(reg))
 
-        self.vals[reg] = val.unsigned()
+        self.vals[reg] = val.signed()
         return True
 
     def get(self, reg: str, mark_read: bool = True) -> Int32:
         """
         Returns the contents of register reg
         :param reg: The register name
         :param mark_read: If the register should be marked as "last read" (only used internally)
```

### Comparing `riscemu-2.2.5/riscemu/core/rtclock.py` & `riscemu-2.2.6/riscemu/core/rtclock.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/simple_instruction.py` & `riscemu-2.2.6/riscemu/core/simple_instruction.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/traps.py` & `riscemu-2.2.6/riscemu/core/traps.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/core/usermode_cpu.py` & `riscemu-2.2.6/riscemu/core/usermode_cpu.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/debug.py` & `riscemu-2.2.6/riscemu/debug.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/decoder/__main__.py` & `riscemu-2.2.6/riscemu/decoder/__main__.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/decoder/decoder.py` & `riscemu-2.2.6/riscemu/decoder/decoder.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/decoder/formats.py` & `riscemu-2.2.6/riscemu/decoder/formats.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/decoder/formatter.py` & `riscemu-2.2.6/riscemu/decoder/formatter.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/decoder/instruction_table.py` & `riscemu-2.2.6/riscemu/decoder/instruction_table.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/helpers.py` & `riscemu-2.2.6/riscemu/helpers.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/instructions/RV32A.py` & `riscemu-2.2.6/riscemu/instructions/RV32A.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/instructions/RV32F.py` & `riscemu-2.2.6/riscemu/instructions/RV32F.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         :Description:
         | Convert a floating-point number in floating-point register rs1 to a signed 32-bit in integer register rd.
 
         :Implementation:
         | x[rd] = sext(s32_{f32}(f[rs1]))
         """
         rd, rs = self.parse_rd_rs(ins)
-        self.regs.set(rd, Int32(int(self.regs.get_f(rs).value)))
+        self.regs.set(rd, Int32.from_float(self.regs.get_f(rs).value))
 
     def instruction_fcvt_wu_s(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+-----+-----+---+
         |31-27|26-25|24-20|19-15|14-12|11-7 |6-2  |1-0|
         +-----+-----+-----+-----+-----+-----+-----+---+
         |11000|00   |00001|rs1  |rm   |rd   |10100|11 |
@@ -51,15 +51,15 @@
         :Description:
         | Convert a floating-point number in floating-point register rs1 to a signed 32-bit in unsigned integer register rd.
 
         :Implementation:
         | x[rd] = sext(u32_{f32}(f[rs1]))
         """
         rd, rs = self.parse_rd_rs(ins)
-        self.regs.set(rd, UInt32(int(self.regs.get_f(rs).value)))
+        self.regs.set(rd, UInt32.from_float((self.regs.get_f(rs).value)))
 
     def instruction_fmv_x_w(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+-----+-----+---+
         |31-27|26-25|24-20|19-15|14-12|11-7 |6-2  |1-0|
         +-----+-----+-----+-----+-----+-----+-----+---+
         |11100|00   |00000|rs1  |000  |rd   |10100|11 |
@@ -91,15 +91,15 @@
         :Description:
         | Converts a 32-bit signed integer, in integer register rs1 into a floating-point number in floating-point register rd.
 
         :Implementation:
         | f[rd] = f32_{s32}(x[rs1])
         """
         rd, rs = self.parse_rd_rs(ins)
-        self.regs.set_f(rd, Float32(self.regs.get(rs).signed().value))
+        self.regs.set_f(rd, Float32(self.regs.get(rs).value))
 
     def instruction_fcvt_s_wu(self, ins: Instruction):
         """
         +-----+-----+-----+-----+-----+-----+-----+---+
         |31-27|26-25|24-20|19-15|14-12|11-7 |6-2  |1-0|
         +-----+-----+-----+-----+-----+-----+-----+---+
         |11010|00   |00001|rs1  |rm   |rd   |10100|11 |
```

### Comparing `riscemu-2.2.5/riscemu/instructions/RV32I.py` & `riscemu-2.2.6/riscemu/instructions/RV32I.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/instructions/RV32M.py` & `riscemu-2.2.6/riscemu/instructions/RV32M.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """
 RiscEmu (c) 2021 Anton Lydike
 
 SPDX-License-Identifier: MIT
 """
 
 from .instruction_set import *
-from riscemu.core.exceptions import INS_NOT_IMPLEMENTED
 
 
 class RV32M(InstructionSet):
     """
     The RV32M Instruction set, containing multiplication and division instructions
     """
 
     def instruction_mul(self, ins: "Instruction"):
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
         self.regs.set(rd, rs1 * rs2)
 
     def instruction_mulh(self, ins: "Instruction"):
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
-        self.regs.set(rd, (rs1 * rs2) >> 32)
+        self.regs.set(rd, Int32((rs1.signed().value * rs2.signed().value) >> 32))
 
     def instruction_mulhsu(self, ins: "Instruction"):
-        INS_NOT_IMPLEMENTED(ins)
+        rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
+        self.regs.set(rd, Int32((rs1.signed().value * rs2.unsigned_value) >> 32))
 
     def instruction_mulhu(self, ins: "Instruction"):
-        INS_NOT_IMPLEMENTED(ins)
+        rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
+        self.regs.set(rd, UInt32((rs1.unsigned_value * rs2.unsigned_value) >> 32))
 
     def instruction_div(self, ins: "Instruction"):
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins)
         self.regs.set(rd, rs1 // rs2)
 
     def instruction_divu(self, ins: "Instruction"):
         rd, rs1, rs2 = self.parse_rd_rs_rs(ins, signed=False)
```

### Comparing `riscemu-2.2.5/riscemu/instructions/RV_Debug.py` & `riscemu-2.2.6/riscemu/instructions/RV_Debug.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/instructions/Zicsr.py` & `riscemu-2.2.6/riscemu/instructions/Zicsr.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/instructions/__init__.py` & `riscemu-2.2.6/riscemu/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/instructions/float_base.py` & `riscemu-2.2.6/riscemu/instructions/float_base.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/instructions/instruction_set.py` & `riscemu-2.2.6/riscemu/instructions/instruction_set.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/interactive.py` & `riscemu-2.2.6/riscemu/interactive.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/libc/README.md` & `riscemu-2.2.6/riscemu/libc/README.md`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/libc/stdlib.s` & `riscemu-2.2.6/riscemu/libc/stdlib.s`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/libc/string.s` & `riscemu-2.2.6/riscemu/libc/string.s`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/priv/CSR.py` & `riscemu-2.2.6/riscemu/priv/CSR.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/priv/ElfLoader.py` & `riscemu-2.2.6/riscemu/priv/ElfLoader.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/priv/ImageLoader.py` & `riscemu-2.2.6/riscemu/priv/ImageLoader.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/priv/PrivCPU.py` & `riscemu-2.2.6/riscemu/priv/PrivCPU.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/priv/PrivMMU.py` & `riscemu-2.2.6/riscemu/priv/PrivMMU.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/priv/PrivRV32I.py` & `riscemu-2.2.6/riscemu/priv/PrivRV32I.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/priv/__main__.py` & `riscemu-2.2.6/riscemu/priv/__main__.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/priv/types.py` & `riscemu-2.2.6/riscemu/priv/types.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/riscemu_main.py` & `riscemu-2.2.6/riscemu/riscemu_main.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/syscall.py` & `riscemu-2.2.6/riscemu/syscall.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/riscemu/tokenizer.py` & `riscemu-2.2.6/riscemu/tokenizer.py`

 * *Files identical despite different names*

### Comparing `riscemu-2.2.5/PKG-INFO` & `riscemu-2.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: riscemu
-Version: 2.2.5
+Version: 2.2.6
 Summary: A basic RISC-V emulator
 Home-page: https://github.com/antonlydike/riscemu
 License: MIT
 Keywords: RISC-V
 Author: Anton Lydike
 Author-email: me@antonlydike.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: importlib-resources (>=6.1.0,<7.0.0)
 Requires-Dist: pyelftools (>=0.30,<0.31)
 Project-URL: Bug Tracker, https://github.com/antonlydike/riscemu/issues
 Project-URL: Repository, https://github.com/antonlydike/riscemu
 Description-Content-Type: text/markdown
 
 # RiscEmu - RISC-V (userspace) emulator in python
@@ -122,7 +123,23 @@
 
 ## TODO:
  * Correctly handle 12 and 20 bit immediate (currently not limited to bits at all)
  * Add a cycle limit to the options and CPU to catch infinite loops
  * Move away from `print` and use `logging.logger` instead
  * Writer proper tests
 
+
+## How To Release:
+
+Create a new commit that:
+1. Changes the "Upcoming" heading to the new versions number
+2. Increments the version in the pyproject.toml to the next version
+
+Commit this, and tag it with `v<version>`. Push the commit and the tag:
+```bash
+git push
+git push origin "v<version>"
+```
+
+On GitHub, [draft a new release](https://github.com/AntonLydike/riscemu/releases/new), and
+then approve the workflow run [here](https://github.com/AntonLydike/riscemu/actions).
+
```

