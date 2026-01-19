# azure
my azure stuff
Repo Struktur

azure-platform/
├── README.md
├── .gitignore
├── .editorconfig

├── docs/
│   ├── architecture.md
│   ├── networking.md
│   └── operations.md

├── infra/
│   ├── terraform/
│   │   ├── modules/
│   │   │   ├── network/
│   │   │   ├── vm/
│   │   │   ├── storage/
│   │   │   └── monitoring/
│   │   ├── envs/
│   │   │   ├── dev/
│   │   │   │   ├── main.tf
│   │   │   │   ├── variables.tf
│   │   │   │   └── terraform.tfvars
│   │   │   ├── prod/
│   │   │   └── test/
│   │   └── versions.tf
│   │
│   └── bicep/
│       └── vm.bicep

├── bootstrap/
│   ├── cloud-init/
│   │   ├── ubuntu.yaml
│   │   └── debian.yaml
│   ├── windows/
│   │   └── bootstrap.ps1
│   └── custom-script/
│       └── install.sh

├── scripts/
│   ├── linux/
│   │   ├── install-docker.sh
│   │   ├── setup-xmrig.sh
│   │   └── hardening.sh
│   ├── windows/
│   │   └── build-env.ps1
│   └── common/
│       └── logging.sh

├── services/
│   ├── systemd/
│   │   └── xmrig.service
│   └── docker/
│       └── docker-compose.yml

├── configs/
│   ├── nginx/
│   ├── bitcoin/
│   ├── monero/
│   └── prometheus/

├── pipelines/
│   ├── github-actions/
│   │   └── deploy.yml
│   └── azure-devops/
│       └── pipeline.yml

└── secrets/
    └── README.md   # leer, erklärt nur wo Secrets liegen
