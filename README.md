# Learning Computer Architecture with Turing Complete / 用 Turing Complete 学习计算机原理

This repository collects what I learn about digital logic and computer architecture by building circuits in *Turing Complete*. The notes focus on the concepts, questions, and experiments that come out of that learning process.

这里记录我借助《Turing Complete》学习数字逻辑与计算机组成时理解的知识点、遇到的问题和动手实践。关卡提供学习的场景，笔记围绕学到的内容展开。

## Notes / 笔记

Notes are grouped by chapter. Within a chapter, an entry can follow a day's learning, explore a concept, or connect a level with the ideas it teaches. Level work and related concepts can stay together in one note.

笔记按章节归档。章节内既可以记录某天的学习进度，也可以围绕一个知识点整理；关卡中的实践与由此学到的原理可以写在同一篇笔记里。

- [第一部分：从与非门开始搭逻辑门](01-布尔代数/从与非门开始搭逻辑门.md)
- [第二部分：算术运算与存储器的前置知识](02-算术运算与存储器/算术运算与存储器的前置知识.md)

## CPU build goals / 处理器构建目标

These are long-term learning goals for sandbox mode, not a fixed schedule. Each core has an explicit instruction set architecture (ISA); its circuit design is a separate question.

以下是沙盒模式中的三个长期学习目标，并非固定进度。每颗核心都有明确的指令集架构（ISA）；具体电路如何实现，需要在设计过程中继续探索。

1. **Hack CPU / Hack 处理器** — Build a 16-bit core for the [Hack ISA](https://www.nand2tetris.org/project05), with separate instruction ROM and data RAM (Harvard architecture). The goal is to run Hack machine-language programs such as Add and Max.

   构建遵循 Hack 指令集的 16 位核心，采用分开的指令 ROM 与数据 RAM（哈佛架构），最终运行 Add、Max 等 Hack 机器语言程序。

2. **RISC-V core / RISC-V 处理器** — Build a 32-bit [RV32I](https://docs.riscv.org/reference/isa/v20260120/unpriv/rv32.html) core. Start without a pipeline, work toward the complete base integer ISA, and treat a five-stage pipeline as a later challenge. The instruction and data paths remain an implementation decision.

   构建 32 位 RV32I 核心：先完成无流水线版本，再逐步覆盖完整的基础整数指令集；五级流水线作为后续挑战。取指与数据访问通路在具体设计时决定。

3. **Armv6-M core / Armv6-M 处理器** — Build a 32-bit core inspired by [Cortex-M0+](https://www.arm.com/-/media/Arm%20Developer%20Community/PDF/Processor%20Datasheets/Arm%20Cortex-M0%20plus%20Processor%20Datasheet.pdf), targeting Armv6-M/Thumb instructions, exceptions, interrupts, and a two-stage pipeline. Follow its shared system-bus (von Neumann) organization; call the result compatible only if that claim is verified.

   以 Cortex-M0+ 为参考，挑战 32 位 Armv6-M/Thumb 核心，逐步实现异常、中断与两级流水线，并参考其共享系统总线的冯·诺依曼组织方式。只有经过充分验证，才称其兼容 Cortex-M0+。

## Language / 语言

The study notes are written primarily in Chinese.

学习笔记以中文为主。

## Coming later / 后续

A more complete, in-depth set of CS:APP study notes is in the works. I'm still studying the material—more to come.

更完整、更深入的 CS:APP 学习笔记正在准备中。我还在深入研读，之后再慢慢展开。

## License / 许可

See [LICENSE](LICENSE). / 见 [LICENSE](LICENSE)。
