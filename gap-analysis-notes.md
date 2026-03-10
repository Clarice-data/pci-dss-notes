# Gap Analysis Notes

## what is a gap analysis?
a gap analysis compares what a business is currently doing against
what PCI-DSS requires. the output is a list of areas where the
business falls short — and a prioritized plan to fix them.

## common gap categories found in small businesses

### 1. policy documentation
most small businesses are doing the right things operationally
but have never written it down. PCI-DSS requires written policies for:
- access control
- incident response
- acceptable use of systems
- password and authentication requirements

**typical fix**: draft simple, plain-language policy documents.
they don't need to be complex — they need to exist and be followed.

### 2. access control
- shared logins across staff members
- no formal process for revoking access when employees leave
- admin credentials not separated from general user credentials

**typical fix**: create individual accounts per user, document
who has access to what, and establish an offboarding checklist.

### 3. network segmentation
- payment systems on the same network as general office equipment
- no firewall rules separating cardholder data from other systems

**typical fix**: work with IT vendor to segment the network or
confirm that payment terminals are fully isolated.

### 4. vendor management
- third-party vendors with access to systems not formally documented
- no review of whether vendors are PCI-compliant themselves

**typical fix**: list all vendors with system access, confirm
each has their own compliance documentation (AOC or SAQ).

### 5. vulnerability management
- no regular process for applying software updates or patches
- antivirus not consistently deployed or monitored

**typical fix**: establish a simple monthly patching checklist
and confirm antivirus coverage on all in-scope systems.

## prioritization approach
gaps were prioritized by:
1. **risk** — how directly does this gap expose cardholder data?
2. **effort** — how quickly can this be fixed with available resources?
3. **documentation vs. technical** — documentation gaps were addressed first
   since they are low-cost and immediately satisfy assessor requirements.

---
*all specific system names, vendor names, and client details have been removed.*
