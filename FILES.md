infrastructure-automation/
├── .env.example
├── requirements.txt
├── infra                           # Executable entry point script
├── main.py                         # Python entry point
├── config/
│   └── defaults.yaml              # Default configurations
├── modules/
│   ├── __init__.py
│   ├── base.py                    # Base classes and interfaces
│   ├── server_manager.py          # Refactored Hetzner server management
│   └── software_setup.py          # Basic software installation module
├── ansible/
│   ├── ansible.cfg
│   ├── inventory/
│   │   └── hosts.yml              # Your Ansible inventory file
│   └── playbooks/
│       ├── common-software.yml    # Basic software setup playbook
│       └── docker-setup.yml       # Docker installation playbook
├── utils/
│   ├── __init__.py
│   ├── config_loader.py           # Configuration management
│   ├── ssh_manager.py             # SSH and known_hosts management
│   └── logger.py                  # Logging utilities
└── logs/                          # Log files directory (created at runtime)