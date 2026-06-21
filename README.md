# Orchestrating Chaos: Defeating Guloader's VEH and Obfuscation with Unicorn

## Workshop at REcon 2026

[https://cfp.recon.cx/recon-2026/talk/Y7Z98G/]()

Standard sandboxes and automated scanners fall short when faced with the modern state of  **Guloader** . Its reliance on **Vectored Exception Handling (VEH)** to redirect control flow through intentional exceptions creates a "black box" for traditional debuggers and linear disassemblers. This 3 hour workshop bypasses the basics and dives straight into the heavy lifting of modern malware deobfuscation.

We will perform a deep-dive dissection of a multi-stage infection chain, moving rapidly through PowerShell loaders into the core of the matter:  **multi-layered shellcode** . Participants will reverse-engineer the "exception soup" of Guloader, mapping out how it uses various CPU instructions and a custom handler to mask its code flow.

The highlight of the session is a transition from manual analysis to  **programmatic automation** . We will leverage the **Unicorn emulator framework** to build a custom configuration extractor capable of reconstructing non-contiguous encrypted payloads that stay hidden from static analysis.
