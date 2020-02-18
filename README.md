# Reproduction of services not receiving events after fast refresh

1. Make any changes
2. Click something in the UI (e.g toggling a TODO)
3. Check the console

You should see an error like the following

```
Warning: Event "TOGGLE_COMPLETE" was sent to stopped service "todo". This service has already reached its final state, and will not transition.
Event: {"type":"TOGGLE_COMPLETE"}
```
