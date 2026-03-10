# PCI-DSS Overview

## what is PCI-DSS?
PCI-DSS (Payment Card Industry Data Security Standard) is a set of security
requirements for any business that accepts, processes, or stores credit card data.
it's maintained by the major card brands (Visa, Mastercard, etc.) and enforced
through annual assessments or self-assessment questionnaires (SAQs).

## why it matters for small businesses
most small businesses assume PCI-DSS only applies to large companies.
in reality, any business that runs a card terminal or takes payments online
is in scope — including small dental practices, retail shops, and service providers.

failing to comply doesn't just mean fines. it means liability if a breach occurs.

## the assessment process
businesses are categorized into "merchant levels" based on transaction volume.
most small businesses fall into Level 4, which requires:
- completing a Self-Assessment Questionnaire (SAQ)
- passing a vulnerability scan (if applicable)
- submitting an Attestation of Compliance (AOC)

## common SAQ types
- **SAQ A** — card data fully outsourced, no electronic storage
- **SAQ B** — standalone terminals, no electronic cardholder data
- **SAQ C** — payment application systems connected to the internet
- **SAQ D** — all other merchants (most complex)

## key takeaway
compliance is mostly about documentation and process.
many businesses are technically doing the right things —
they just haven't documented it in a way that satisfies an assessor.

---
*this document is a plain-language summary based on direct experience
coordinating a PCI-DSS remediation. it is not a substitute for official PCI guidance.*
