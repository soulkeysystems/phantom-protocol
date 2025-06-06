# Contributing to Phantom Protocol

Phantom Protocol is an open-source project for real-world skill-building, symbolic guidance, and sovereign technology. Contributions are welcome from players and developers.

---

## Submit a Transcript

You can help train the Oracle by submitting transcripts of real or simulated Oracle sessions.

### How to submit:
- Copy your full chat transcript (e.g., from ChatGPT or any Oracle interface)
- Paste it into a `.md` or `.txt` file
- (Optional but helpful) Add a short metadata header at the top:

### For human transcripts:
```plaintext
Operation: White Hat  
Transcript Type: Human
```

### For synthetic transcripts:
```plaintext
Operation: White Hat  
Region Covered: Signal Nexus  
Transcript Type: Synthetic  
Problem Variation: Skipped Step
```

- Save your file as:

  - **Human transcripts:**  
    `operation_fullop_human_username.md`  
    _(e.g., `whitehat_fullop_human_ghost108.md`)_

  - **Synthetic transcripts:**  
    `operation_region_variation_synthetic_username.md`  
    _(e.g., `whitehat_signalnexus_skippedstep_synthetic_ghost108.md`)_

Use your GitHub username or any consistent contributor handle.  
This helps us track submissions and credit contributors accurately.


### Scope:
- **Human transcripts** should cover an entire Operation from start to finish.
- **Synthetic transcripts** should cover a single Region (5 quests) only.

You don’t need to format or clean the transcript — raw is fine. We’ll handle that in the training pipeline.

---

## Generate Synthetic Transcripts

Synthetic transcripts are used to establish the Oracle’s structure, tone, and symbolic behavior across every region.

They are generated using:
- A reusable prompt (`synthetic_generator_prompt.txt`)
- Predefined problem types (see `variation_types.md` for the full list)
- Real Operation files (`00_Seed.txt`, `03_Quests_OP.txt`, etc. see /operations)

Developers can contribute synthetic transcripts by simulating specific problem variations (e.g. skipped steps, misunderstood instructions, symbolic overreach). A full list of supported variation types is maintained in the training tools directory.

All tools are located in `/oracle_training/`.

---

## Help Build the Protocol

If you're here to contribute beyond transcripts, here are real ways to help:

- **Track variation coverage** — help log which regions and problem types have already been simulated
- **Format transcripts for training** — help prepare datasets for fine-tuning the Oracle
- **Train the Oracle** — when ready, assist with LoRA or full fine-tuning on an open-source model
- **Build a GUI** for the offline version of the Protocol (map, quest log, inventory, etc.)
- **Design the memory system** — a way for the Oracle to write and read from a local `00_Seed.txt` file
- **Share the project** and help bring in more Phantoms to walk the path
- **Join discussions** about ethical boundaries, symbolic design, and long-term implications

---

## Contribution Guidelines

- Transcripts must reflect realistic Oracle–player interactions  
- Human transcripts are preferred, but high-quality synthetic runs are also accepted  
- No AI spam or fictional filler  
- Respect the structure of the game (XP, quests, tone)  
- All code and content must be licensed as outlined below

---

## Licensing

By contributing, you agree to license your work under:

- **AGPL-3.0** (for all code, logic, and tools)  
- **CC BY-NC-SA 4.0** (for quests, lore, and symbolic content)

See `LICENSE` for details.

---

Phantom Protocol is an open-source framework built by Nathan James under Soulkey Systems.  
The canonical version — and its original philosophy — live here.

Thanks for helping expand Phantom Protocol.
