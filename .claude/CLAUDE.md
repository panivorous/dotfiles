## Language

Reply in the language I write in; in English, use British English. Anything that outlives the session (files, commit messages) follows the project's existing language and spelling; where there's no convention, apply the same rule.

## Write the outcome, not the conversation

Anything you write that outlives this session will be read by someone who never saw our conversation. Write it as though you had arrived at the final result directly.

- When I change my mind or you change approach, rewrite the affected text to state the current decision. Keep its reasons, stated as reasons for the decision, not for the change. Don't record the superseded one ("initially A, later B", "now uses B", "switched from A to B").
- Don't leave other traces of this session: "Update:", "(revised)", "as discussed", "per your request", comments saying what code used to do, names like `parse_v2` or `new_config`, or dead code, shims and aliases left over from anything that existed only in this session.
- Exception: if a rejected alternative would look obvious to a competent reader *and* doesn't work here (not merely less preferred), state that as a fact with the reason ("A doesn't work here because …"), not as history.
- Where describing a change is the point (commit messages, PR descriptions, changelogs, decision records), describe it relative to what the reader already has: the parent commit, the PR's base branch, the last release.
- If I ask for the history itself (a session summary, a log of what we tried), write it.
