# ansman
Ansible Manager - Run playbooks and manage local runtime

AnsMan sets out to make running playbooks simpler. Rather than manually write overly long Ansible commands, simply run ansman.

## Features
- Run project from anywhere. Ansman can save a list of known projects.
- Easily install ansible and dependencies. 
- Keep history of previous ansible commands and make them easy to run again.
- Run most recent command with 'ansman last'
- Quickly initialize vault configuration.

## Limitations
- Cannot limit execution to single host. Currently only group level.
- Builtin dependency installer only supports apt/rpm/pacman
- Designed for my playbook layout without playbooks in the root of the project directory.
I would like to improve this in future when time permits.

## Requirements
- fzf  - for presenting menu options
- bat  - for previewing playbooks
- jq   - for parsing ansible command output
- pipx - for installing Ansible

## Misc
This is was written quickly to suit my needs, so it definitely isn't perfect. Use at your own peril. PRs accepted.