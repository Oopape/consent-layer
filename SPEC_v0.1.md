# Consent Layer Standard v0.1

## Scope
Applies to AI actions affecting the real world:
• Money
• Messaging
• Bookings

## Consent requirements
1. Present clear action summary
2. Require explicit phrase:
   I confirm. Execute now.
3. Log consent proof (voice, text, or tap)
4. Emit receipt
5. Provide undo window (120 mins default)
6. Pause if emotional state detected
7. Always obey: Stop. Do not execute.

## State model
Listen → Propose → Confirm → Execute → Receipt → Undo window → Closed

Forbidden:
• Listen → Execute
• Propose → Execute (for high-impact actions)
• Any → Execute during emotional hold

## Undo window
Default: 120 minutes

## Receipt format
version  
action_id  
action_summary  
consent_mode  
consent_evidence_hash  
timestamp  
undo_window_expires  
policy_version  

## Principle
Human will is the root authority.  
AI must earn execution through clarity and reversibility.
