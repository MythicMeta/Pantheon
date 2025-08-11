# Pantheon
*A collection of eventing scripts for Mythic C2, which also includes resources to build your own*

## 🏛️ Overview
Pantheon is a repository containing eventing automation which include reconnaissance, persistance location, and credential preparation scripts.

## File Naming Convention

All files follow a standardized naming pattern for easy identification:
```
[RISK-LEVEL]_[DESCRIPTIVE-NAME]_[PAYLOAD-TYPE].yaml
```

### Risk Levels
- **LOW**: Minimal detection risk, safe for routine operations
- **MEDIUM**: Moderate detection risk, use with awareness
- **HIGH**: High detection risk, use with extreme caution


### Examples
- `LOW_NetworkHostRecon_Apollo.yaml`
- `HIGH_TicketDump_Apollo.yaml`
- `MEDIUM_ServiceRecon_Apollo.yaml`

## OPSEC Considerations

- Always review risk levels before deployment
- HIGH risk events should only be used in approved test environments or with explicit authorization
- Consider beacon callback timing for automated event chains
- BOFs may require specific file uploads before execution

## Usage Guidelines

1. **Event Selection**: Choose events based on operation phase and risk tolerance
2. **Payload Compatibility**: Ensure events match your payload type
3. **Dependency Management**: Some events depend on other paths or resource locations to continue
4. **Error Handling**: Monitor for execution errors and adjust beacon timing if needed

## BOF Management

- BOF files referenced in events must be registered to the agent before execution
---
