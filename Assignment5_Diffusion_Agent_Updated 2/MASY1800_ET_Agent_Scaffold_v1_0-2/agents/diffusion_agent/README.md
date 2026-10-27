# Diffusion agent

Assignment 5 specialist built on the unchanged MASY1800 frozen core. The specialist is **technology-neutral**: it analyzes the technology, application, organization, and adoption posture supplied in its input. **Generative-AI coding assistants are the illustrative primary and contrast test technology**, not a hard-coded restriction. The assignment does not prescribe a particular technology. If the instructor or team specifies another technology, replace the test cases and verify corresponding evidence before submission.

From the scaffold directory:

```bash
python tools/check_frozen_core.py
python tools/build_prompt.py --agent agents/diffusion_agent --case agents/diffusion_agent/cases/primary.json
python tools/build_prompt.py --agent agents/diffusion_agent --case agents/diffusion_agent/cases/contrast_1.json
python tools/build_prompt.py --agent agents/diffusion_agent --case agents/diffusion_agent/cases/contrast_2.json
python tools/validate_response.py agents/diffusion_agent/responses/primary_response.json
python tools/validate_response.py agents/diffusion_agent/responses/contrast_1_response.json
python tools/validate_response.py agents/diffusion_agent/responses/contrast_2_response.json
```

Prompt packets are intended for ChatGPT; no API key is required. The preserved responses are analytical example runs grounded in the dated source notes, **not independent live deployment data**. The basic validator checks types/required fields, not evidence validity or intellectual quality. Read `records/agent_record.md` and `records/evidence_notes.md` before reuse.
