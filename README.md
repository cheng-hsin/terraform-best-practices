# terraform-best-practices

terraform-best-practices/
├── modules/                # 放置可重用的元件
│   └── network/
│       ├── main.tf
│       ├── variables.tf
│       └── outputs.tf
├── environments/           # 區分開發與生產環境
│   └── dev/
│       ├── main.tf         # 呼叫 modules
│       ├── providers.tf    # 定義 LocalStack 連線
│       └── terraform.tfvars # 環境專屬變數
└── .gitignore              # 排除敏感檔案 (如 .tfstate)
