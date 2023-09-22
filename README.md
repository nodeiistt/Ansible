# Cosmos-based Node Ansible Setup Plus Several Supporting Playbooks

## Design Philosophy

1. Extendable to most Tendermint-based chains
1. Support both mainnet and testnet
1. Stable playbooks and roles; Customizable variables
1. Support essential functions (snapshot, state-sync, public RPC/API endpoints) through separate playbooks

## TL/DR

You run one playbook and set up a node.

```bash
ansible-playbook main.yml -e "target=ununifi_main"
ansible-playbook -i inventory_testnet.ini main.yml -e "target=ununifi_test"
```
