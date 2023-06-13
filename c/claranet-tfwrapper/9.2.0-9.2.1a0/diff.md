# Comparing `tmp/claranet-tfwrapper-9.2.0.tar.gz` & `tmp/claranet-tfwrapper-9.2.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claranet-tfwrapper-9.2.0.tar", max compression
+gzip compressed data, was "claranet-tfwrapper-9.2.1a0.tar", max compression
```

## Comparing `claranet-tfwrapper-9.2.0.tar` & `claranet-tfwrapper-9.2.1a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    16725 2022-02-08 08:32:39.897772 claranet-tfwrapper-9.2.0/LICENSE
--rw-r--r--   0        0        0    22619 2022-02-08 08:32:39.897772 claranet-tfwrapper-9.2.0/README.md
--rw-r--r--   0        0        0     2316 2022-02-08 08:32:39.897772 claranet-tfwrapper-9.2.0/pyproject.toml
--rwxr-xr-x   0        0        0    68594 2022-02-08 08:32:39.897772 claranet-tfwrapper-9.2.0/src/claranet_tfwrapper/__init__.py
--rw-r--r--   0        0        0      205 2022-02-08 08:32:39.897772 claranet-tfwrapper-9.2.0/src/claranet_tfwrapper/utils.py
--rw-r--r--   0        0        0    24921 2022-02-08 08:32:49.913558 claranet-tfwrapper-9.2.0/setup.py
--rw-r--r--   0        0        0    24549 2022-02-08 08:32:49.915489 claranet-tfwrapper-9.2.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2022-02-10 10:29:34.477640 claranet-tfwrapper-9.2.1a0/LICENSE
+-rw-r--r--   0        0        0    22619 2022-02-10 10:29:34.477640 claranet-tfwrapper-9.2.1a0/README.md
+-rw-r--r--   0        0        0     2363 2022-02-10 10:29:34.477640 claranet-tfwrapper-9.2.1a0/pyproject.toml
+-rwxr-xr-x   0        0        0    68594 2022-02-10 10:29:34.477640 claranet-tfwrapper-9.2.1a0/src/claranet_tfwrapper/__init__.py
+-rw-r--r--   0        0        0      205 2022-02-10 10:29:34.477640 claranet-tfwrapper-9.2.1a0/src/claranet_tfwrapper/utils.py
+-rw-r--r--   0        0        0    24923 2022-02-10 10:29:43.323686 claranet-tfwrapper-9.2.1a0/setup.py
+-rw-r--r--   0        0        0    24551 2022-02-10 10:29:43.325474 claranet-tfwrapper-9.2.1a0/PKG-INFO
```

### Comparing `claranet-tfwrapper-9.2.0/LICENSE` & `claranet-tfwrapper-9.2.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `claranet-tfwrapper-9.2.0/README.md` & `claranet-tfwrapper-9.2.1a0/README.md`

 * *Files identical despite different names*

### Comparing `claranet-tfwrapper-9.2.0/pyproject.toml` & `claranet-tfwrapper-9.2.1a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "claranet-tfwrapper"
-version = "9.2.0"
+version = "9.2.1-alpha.0"
 description = "Claranet's `tfwrapper` is a wrapper for [Terraform](https://www.terraform.io/) implemented in python which aims to simplify Terraform usage and enforce best practices"
 authors = []
 license = "Mozilla Public License Version 2.0"
 readme = "README.md"
 homepage = "https://github.com/claranet/terraform-wrapper"
 keywords = ["terraform", "wrapper"]
 
@@ -25,20 +25,20 @@
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.6.2,<4.0"
 boto3 = "^1.17.94"
 CacheControl = "^0.12.6"
-colorlog = "^5.0.1"
+colorlog = ">=5.0.1,<7.0.0"
 Jinja2 = "^3.0.1"
 lockfile = "^0.12.2"
-natsort = "^7.1.1"
+natsort = ">=7.1.1,<9.0.0"
 packaging = "^21.0"
-PyYAML = "^5.4.1"
+PyYAML = ">=5.4.1,<7.0.0"
 requests = "^2.25.1"
 schema = "^0.7.4"
 termcolor = "^1.1.0"
 
 azure-cli-core = {version = "^2.30.0", optional = true}
 azure-common = {version = "^1.1.27", optional = true}
 azure-mgmt-storage = {version = "^18.0.0", optional = true}
@@ -50,22 +50,23 @@
   "azure-cli-core",
   "azure-common",
   "azure-mgmt-storage",
   "msrestazure",
 ]
 
 [tool.poetry.dev-dependencies]
-black = "^21.7b0"
-md-toc = "^8.0.0"
-flake8 = "^3.9.2"
+black = "^22.1"
+md-toc = "^8.1.1"
+flake8 = "^4.0.1"
 flake8-docstrings = "^1.6.0"
 mock = "^4.0.3"
 pook = "^1.0.2"
-pytest = "^6.2.4"
+pytest = "^7.0.0"
 requests-mock = "^1.9.3"
+toml = "^0.10.2"
 
 [tool.poetry.scripts]
 tfwrapper = 'claranet_tfwrapper:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `claranet-tfwrapper-9.2.0/src/claranet_tfwrapper/__init__.py` & `claranet-tfwrapper-9.2.1a0/src/claranet_tfwrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `claranet-tfwrapper-9.2.0/setup.py` & `claranet-tfwrapper-9.2.1a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['CacheControl>=0.12.6,<0.13.0',
  'Jinja2>=3.0.1,<4.0.0',
- 'PyYAML>=5.4.1,<6.0.0',
+ 'PyYAML>=5.4.1,<7.0.0',
  'argcomplete<2.0',
  'boto3>=1.17.94,<2.0.0',
- 'colorlog>=5.0.1,<6.0.0',
+ 'colorlog>=5.0.1,<7.0.0',
  'lockfile>=0.12.2,<0.13.0',
- 'natsort>=7.1.1,<8.0.0',
+ 'natsort>=7.1.1,<9.0.0',
  'packaging>=21.0,<22.0',
  'requests>=2.25.1,<3.0.0',
  'schema>=0.7.4,<0.8.0',
  'termcolor>=1.1.0,<2.0.0']
 
 extras_require = \
 {'azure': ['azure-cli-core>=2.30.0,<3.0.0',
@@ -31,15 +31,15 @@
            'msrestazure>=0.6.4,<0.7.0']}
 
 entry_points = \
 {'console_scripts': ['tfwrapper = claranet_tfwrapper:main']}
 
 setup_kwargs = {
     'name': 'claranet-tfwrapper',
-    'version': '9.2.0',
+    'version': '9.2.1a0',
     'description': "Claranet's `tfwrapper` is a wrapper for [Terraform](https://www.terraform.io/) implemented in python which aims to simplify Terraform usage and enforce best practices",
     'long_description': '# claranet-tfwrapper\n\n[![Changelog](https://img.shields.io/badge/changelog-release-blue.svg)](CHANGELOG.md) [![Mozilla Public License](https://img.shields.io/badge/license-mozilla-orange.svg)](LICENSE) [![Pypi](https://img.shields.io/badge/python-pypi-green.svg)](https://pypi.org/project/claranet-tfwrapper/)\n\n`tfwrapper` is a python wrapper for [Terraform](https://www.terraform.io/) which aims to simplify Terraform usage and enforce best practices.\n\n## Table Of Contents\n\n<!--TOC-->\n\n- [claranet-tfwrapper](#claranet-tfwrapper)\n  - [Table Of Contents](#table-of-contents)\n  - [Features](#features)\n  - [Drawbacks](#drawbacks)\n  - [Setup Dependencies](#setup-dependencies)\n  - [Runtime Dependencies](#runtime-dependencies)\n  - [Recommended setup](#recommended-setup)\n  - [Installation](#installation)\n  - [Setup command-line completion](#setup-command-line-completion)\n  - [Upgrade from tfwrapper v7 or older](#upgrade-from-tfwrapper-v7-or-older)\n    - [Required files](#required-files)\n  - [Configuration](#configuration)\n    - [tfwrapper configuration](#tfwrapper-configuration)\n    - [Stacks configurations](#stacks-configurations)\n    - [States centralization configuration](#states-centralization-configuration)\n    - [How to migrate from one backend to another for state centralization](#how-to-migrate-from-one-backend-to-another-for-state-centralization)\n  - [Stacks file structure](#stacks-file-structure)\n  - [Usage](#usage)\n    - [Stack bootstrap](#stack-bootstrap)\n    - [Working on stacks](#working-on-stacks)\n    - [Passing options](#passing-options)\n  - [Environment](#environment)\n    - [S3 state backend credentials](#s3-state-backend-credentials)\n    - [Azure storage state backend credentials](#azure-storage-state-backend-credentials)\n    - [Azure Service Principal credentials](#azure-service-principal-credentials)\n    - [GCP configuration](#gcp-configuration)\n    - [GKE configurations](#gke-configurations)\n    - [Stack configurations and credentials](#stack-configurations-and-credentials)\n    - [Stack path](#stack-path)\n- [Development](#development)\n  - [Tests](#tests)\n  - [Debug command-line completion](#debug-command-line-completion)\n  - [Python code formatting](#python-code-formatting)\n  - [Checks](#checks)\n  - [README TOC](#readme-toc)\n  - [Using terraform development builds](#using-terraform-development-builds)\n  - [git pre-commit hooks](#git-pre-commit-hooks)\n  - [Tagging and publishing new releases to PyPI](#tagging-and-publishing-new-releases-to-pypi)\n\n<!--TOC-->\n\n## Features\n\n- Terraform behaviour overriding\n- State centralization enforcement\n- Standardized file structure\n- Stack initialization from templates\n- AWS credentials caching\n- Azure credentials loading (both Service Principal or User)\n- GCP and GKE user ADC support\n- Plugins caching\n- Tab completion\n\n## Drawbacks\n\n- AWS oriented (even if other cloud providers do work)\n- Setup overhead\n\n## Setup Dependencies\n\n- `build-essential` (provides C/C++ compilers)\n- `libffi-dev`\n- `libssl-dev`\n- `python3` `>= 3.6.2 <4.0` (3.8+ recommended)\n- `python3-dev`\n- `python3-venv`\n\n## Runtime Dependencies\n\n- `terraform` `>= 0.10`\n- `azure-cli` `>= 2.30.0` when using `[azure]` extras\n\n## Recommended setup\n\n- Terraform 1.0+\n- An AWS S3 bucket and DynamoDB table for state centralization in AWS.\n- An Azure Blob Storage container for state centralization in Azure.\n\n## Installation\n\ntfwrapper should installed using pipx (recommended) or pip:\n\n```bash\npipx install claranet-tfwrapper\n```\n\nIf targeting Azure, you should instead install `claranet-tfwrapper` with its `azure` extras:\n\n```bash\npipx install claranet-tfwrapper[azure]\n```\n\nWith zsh, you need to escape brackets:\n\n```zsh\npipx install \'claranet-tfwrapper[azure]\'\n```\n\n## Setup command-line completion\n\nAdd the following to your shell\'s interactive configuration file, e.g. `.bashrc` for bash:\n\n```bash\neval "$(register-python-argcomplete tfwrapper -e tfwrapper)"\n```\n\nYou can then press the completion key (usually `Tab ↹`) twice to get your partially typed `tfwrapper` commands completed.\n\nNote: the `-e tfwrapper` parameter adds an suffix to the defined `_python_argcomplete` function to avoid clashes with other packages (see https://github.com/kislyuk/argcomplete/issues/310#issuecomment-697168326 for context).\n\n## Upgrade from tfwrapper v7 or older\n\nIf you used versions of the wrapper older than v8, there is not much to do when upgrading to v8\nexcept a little cleanup.\nIndeed, the wrapper is no longer installed as a git submodule of your project like it used to be instructed and there is no longer any `Makefile` to activate it.\n\nJust clean up each project by destroying the `.wrapper` submodule:\n\n```bash\ngit rm -f Makefile\ngit submodule deinit .wrapper\nrm -rf .git/modules/.wrapper\ngit rm -f .wrapper\n```\n\nThen check the staged changes and commit them.\n\n### Required files\n\ntfwrapper expects multiple files and directories at the root of a project.\n\n#### conf\n\nStacks configurations are stored in the `conf` directory.\n\n#### templates\n\nThe `templates` directory is used to store the state backend configuration template and the Terraform stack templates used to initialize new stacks. Using a git submodule is recommended.\n\nThe following files are required:\n\n- `templates/{provider}/common/state.tf.jinja2`: AWS S3 or Azure Blob Storage state backend configuration template.\n- `templates/{provider}/basic/main.tf`: the default Terraform configuration for new stacks. The whole `template/{provider}/basic` directory is copied on stack initialization.\n\nFor example with AWS:\n\n```bash\nmkdir -p templates/aws/common templates/aws/basic\n\n# create state configuration template with AWS backend\ncat << \'EOF\' > templates/aws/common/state.tf.jinja2\n{% if region is not none %}\n{% set region = \'/\' + region + \'/\' %}\n{% else %}\n{% set region = \'/\' %}\n{% endif %}\n\nterraform {\n  backend "s3" {\n    bucket = "my-centralized-terraform-states-bucket"\n    key    = "{{ client_name }}/{{ account }}/{{ environment }}{{ region }}{{ stack }}/terraform.state"\n    region = "eu-west-1"\n\n    lock_table = "my-terraform-states-lock-table"\n  }\n}\n\nresource "null_resource" "state-test" {}\nEOF\n\n# create a default stack templates with support for AWS assume role\ncat << \'EOF\' > templates/aws/basic/main.tf\nprovider "aws" {\n  region     = "${var.aws_region}"\n  access_key = "${var.aws_access_key}"\n  secret_key = "${var.aws_secret_key}"\n  token      = "${var.aws_token}"\n}\nEOF\n```\n\nFor example with Azure:\n\n```bash\nmkdir -p templates/azure/common templates/azure/basic\n\n# create state configuration template with Azure backend\ncat << \'EOF\' > templates/azure/common/state.tf.jinja2\n{% if region is not none %}\n{% set region = \'/\' + region + \'/\' %}\n{% else %}\n{% set region = \'/\' %}\n{% endif %}\n\nterraform {\n  backend "azurerm" {\n    storage_account_name = "my-centralized-terraform-states-account"\n    container_name       = "terraform-states"\n\n    key = "{{ client_name }}/{{ account }}/{{ environment }}{{ region }}{{ stack }}/terraform.state"\n  }\n}\nEOF\n\n# create a default stack templates with support for Azure credentials\ncat << \'EOF\' > templates/azure/basic/main.tf\nprovider "azurerm" {\n  subscription_id = "${var.azure_subscription_id}"\n  tenant_id       = "${var.azure_tenant_id}"\n}\nEOF\n```\n\n#### .run\n\nThe `.run` directory is used for credentials caching and plan storage.\n\n```bash\nmkdir .run\ncat << \'EOF\' > .run/.gitignore\n*\n!.gitignore\nEOF\n```\n\n#### .gitignore\n\nAdding the following `.gitignore` at the root of your project is recommended:\n\n```bash\ncat << \'EOF\' > .gitignore\n*/**/terraform.tfstate\n*/**/terraform.tfstate.backup\n*/**/terraform.tfvars\n*/**/.terraform/modules\n*/**/.terraform/plugins\nEOF\n```\n\n## Configuration\n\ntfwrapper uses yaml files stored in the `conf` directory of the project.\n\n### tfwrapper configuration\n\ntfwrapper uses some default behaviors that can be overridden or modified via a `config.yml` file in the `conf` directory.\n\n```yaml\n---\ninstall_azure_dependencies: True # Install all needed Azure dependencies in the loaded shell (azure-cli, azure python SDK)\nalways_trigger_init: False # Always trigger `terraform init` first when launching `plan` or `apply` commands\npipe_plan_command: "cat" # Default command used when you\'re invoking tfwrapper with `--pipe-plan`\nuse_local_azure_session_directory: False # Use the current user\'s Azure configuration in `~/.azure`. By default, the wrapper stores `azure-cli` session and configuration in the local `.run` directory.\n```\n\n### Stacks configurations\n\nStacks configuration files use the following naming convention:\n\n```bash\nconf/${account}_${environment}_${region}_${stack}.yml\n```\n\nHere is an example for an AWS stack configuration:\n\n```yaml\n---\nstate_configuration_name: "aws" # use "aws" backend state configuration\naws:\n  general:\n    account: &aws_account "xxxxxxxxxxx" # aws account for this stack\n    region: &aws_region eu-west-1 # aws region for this stack\n  credentials:\n    profile: my-aws-profile # should be configured in .aws/config\n\nterraform:\n  vars: # variables passed to terraform\n    aws_account: *aws_account\n    aws_region: *aws_region\n    client_name: my-client-name # arbitrary client name\n```\n\nHere is an example for a stack on Azure configuration using user mode and AWS S3 backend for state storage:\n\n```yaml\n---\nstate_configuration_name: "aws-demo" # use "aws" backend state configuration\nazure:\n  general:\n    mode: user # Uses personal credentials with MFA\n    directory_id: &directory_id "aaaaaaaa-bbbb-cccc-dddd-zzzzzzzzzzzz" # Azure Tenant/Directory UID\n    subscription_id: &subscription_id "aaaaaaaa-bbbb-cccc-dddd-zzzzzzzzzzzz" # Azure Subscription UID\n\nterraform:\n  vars:\n    subscription_id: *subscription_id\n    directory_id: *directory_id\n    client_name: client-name #Replace it with the name of your client\n    #version: "0.10"  # Terraform version like "0.10" or "0.10.5" - optional\n```\n\nIt is using your account linked to a Microsoft Account. You must have access to the Azure Subscription if you want to use Terraform.\n\nHere is an example for a stack on Azure configuration using Service Principal mode:\n\n```yaml\n---\nazure:\n  general:\n    mode: service_principal # Uses an Azure tenant Service Principal account\n    directory_id: &directory_id "aaaaaaaa-bbbb-cccc-dddd-zzzzzzzzzzzz" # Azure Tenant/Directory UID\n    subscription_id: &subscription_id "aaaaaaaa-bbbb-cccc-dddd-zzzzzzzzzzzz" # Azure Subscription UID\n\n  credential:\n    profile: azurerm-account-profile # To stay coherent, create an AzureRM profile with the same name than the account-alias. Please checkout `azurerm_config.yml.sample` file for configuration structure.\n\nterraform:\n  vars:\n    subscription_id: *subscription_id\n    directory_id: *directory_id\n    client_name: client-name # Replace it with the name of your client\n    #version: "0.10"  # Terraform version like "0.10" or "0.10.5" - optional\n```\n\nIt is using the Service Principal\'s credentials to connect the Azure Subscription. This SP must have access to the subscription.\nThe wrapper loads client_id and client_secret from your `config.yml` located in `~/.azurem/config.yml`.\n`~/.azurem/config.yml` file structure example:\n\n```yaml\n# File located at ~/.azurerm/config.yml\n\nclaranet-sandbox:\n  client_id: aaaaaaaa-bbbb-cccc-dddd-zzzzzzzzzzzz\n  client_secret: AAbbbCCCzzz==\n\ncustomer-profile:\n  client_id: aaaaaaaa-bbbb-cccc-dddd-zzzzzzzzzzzz\n  client_secret: AAbbbCCCzzz==\n```\n\nHere is an example for a GCP/GKE stack with user ADC and multiple GKE instances:\n\n```yaml\n---\ngcp:\n  general:\n    mode: adc-user\n    project: &gcp_project project-name\n  gke:\n    - name: kubernetes-1\n      zone: europe-west1-c\n    - name: kubernetes-2\n      region: europe-west1\n\nterraform:\n  vars:\n    gcp_region: europe-west1\n    gcp_zone: europe-west1-c\n    gcp_project: *gcp_project\n    client_name: client-name\n    #version: "0.11"  # Terraform version like "0.10" or "0.10.5" - optional\n```\n\n### States centralization configuration\n\nThe `conf/state.yml` configuration file defines the configurations used to connect to state backend account.\nIt can be an AWS (S3) or Azure (Storage Account) backend type.\n\nYou can use other backends (e.g. Google GCS or Hashicorp Consul) not specifically supported by the wrapper if you them manage yourself and omit the `conf/state.yml` file or make it empty:\n\n```yaml\n---\n```\n\nExample configuration with both AWS and Azure backends defined:\n\n```yaml\n---\naws:\n  name: "aws-demo"\n  general:\n    account: "xxxxxxxxxxx"\n    region: eu-west-1\n  credentials:\n    profile: my-state-aws-profile # should be configured in .aws/config\n\nazure:\n  name: "azure-alternative"\n  general:\n    subscription_uid: "xxxxxxx" # the Azure account to use for state storage\n    resource_group_name: "tfstates-xxxxx-rg" # The Azure resource group with state storage\n    storage_account_name: "tfstatesxxxxx"\n\nbackend_parameters: # Parameters or options which can be used by `state.j2.tf` template file\n  state_snaphot: "false" # Example of Azure storage backend option\n```\n\nNote: the first backend will be the default one for stacks not defining `state_backend_type`.\n\n### How to migrate from one backend to another for state centralization\n\nIf for example you have both an AWS and Azure state backend configured in your `conf/state.yml` file,\nyou can migrate your stack state from one backend to another.\n\nHere is a quick howto:\n\n1. Make sure your stack is clean:\n\n```bash\n$ cd account/path/env/your_stack\n$ tfwrapper init\n$ tfwrapper plan\n# should return no changes\n```\n\n2. Change your backend in the stack configuration yaml file:\n\n```yaml\n---\n#state_configuration_name: \'aws-demo\' # previous backend\nstate_configuration_name: "azure-alternative" # new backend to use\n```\n\n3. Back in your stack directory, you can perform the change:\n\n```bash\n$ cd account/path/env/your_stack\n$ rm -v state.tf # removing old state backend configuration\n$ tfwrapper bootstrap # regen a new state backend configuration based on the stack yaml config file\n$ tfwrapper init # Terraform will detect the new backend and propose to migrate it\n$ tfwrapper plan\n# should return the same changes diff as before\n```\n\n## Stacks file structure\n\nTerraform stacks are organized based on their:\n\n- account: an account alias which may reference one or multiple providers accounts. `aws-production`, `azure-dev`, etc…\n- environment: `production`, `preproduction`, `dev`, etc…\n- region: `eu-west-1`, `westeurope`, `global`, etc…\n- stack: defaults to `default`. `web`, `admin`, `tools`, etc…\n\nThe following file structure is enforced:\n\n```\n# enforced file structure\n└── account\n    └── environment\n        └── region\n            └── stack\n\n# real-life example\n├── aws-account-1\n│\xa0\xa0 └── production\n│\xa0\xa0     ├── eu-central-1\n│\xa0\xa0     │\xa0\xa0 └── web\n│\xa0\xa0     │\xa0\xa0     └── main.tf\n│\xa0\xa0     └── eu-west-1\n│\xa0\xa0         ├── default\n│\xa0\xa0         │\xa0\xa0 └── main.t\n│\xa0\xa0         └── tools\n│\xa0\xa0             └── main.tf\n└── aws-account-2\n    └── backup\n        └── eu-west-1\n            └── backup\n                └── main.tf\n```\n\n## Usage\n\n### Stack bootstrap\n\nAfter creating a `conf/${account}_${environment}_${region}_${stack}.yml` stack configuration file you can bootstrap it.\n\n```bash\n# you can bootstrap using the templates/{provider}/basic stack\ntfwrapper -a ${account} -e ${environment} -r ${region} -s ${stack} bootstrap\n\n# or another stack template, for example: templates/aws/foobar\ntfwrapper -a ${account} -e ${environment} -r ${region} -s ${stack} bootstrap aws/foobar\n```\n\n### Working on stacks\n\nYou can work on stacks from their directory or from the root of the project.\n\n```bash\n# working from the root of the project\ntfwrapper -a ${account} -e ${environment} -r ${region} -s ${stack} plan\n\n# working from the root of a stack\ncd ${account}/${environment}/${region}/${stack}\ntfwrapper plan\n```\n\nYou can also work on several stacks sequentially with the `foreach` subcommand from any directory under the root of the project.\nBy default, `foreach` selects all stacks under the current directory,\nso if called from the root of the project without any filter,\nit will select all stacks and execute the specified command in them, one after another:\n\n```bash\n# working from the root of the project\ntfwrapper foreach -- tfwrapper init\n```\n\nAny combination of the `-a`, `-e`, `-r` and `-s` arguments can be used to select specific stacks,\ne.g. all stacks for an account across all environments but in a specific region:\n\n```bash\n# working from the root of the project\ntfwrapper -a ${account} -r ${region} foreach -- tfwrapper plan\n```\n\nThe same can be achieved with:\n\n```bash\n# working from an account directory\ncd ${account}\ntfwrapper -r ${region} foreach -- tfwrapper plan\n```\n\nComplex commands can be executed in a sub-shell with the `-c` argument, e.g.:\n\n```bash\n# working from an environment directory\ncd ${account}/${environment}\ntfwrapper foreach -c \'pwd && tfwrapper init >/dev/null 2>&1 && tfwrapper plan 2>/dev/null -- -no-color | grep "^Plan: "\'\n```\n\n### Passing options\n\nYou can pass anything you want to `terraform` using `--`.\n\n```bash\ntfwrapper plan -- -target resource1 -target resource2\n```\n\n## Environment\n\ntfwrapper sets the following environment variables.\n\n### S3 state backend credentials\n\nThe default AWS credentials of the environment are set to point to the S3 state backend. Those credentials are acquired from the profile defined in `conf/state.yml`\n\n- `AWS_ACCESS_KEY_ID`\n- `AWS_SECRET_ACCESS_KEY`\n- `AWS_SESSION_TOKEN`\n\n### Azure storage state backend credentials\n\nWhen using Azure storage (container blob), needed credentials are set in the environment. Those credentials are acquired from the profile defined in `conf/state.yml`\n\n- `ARM_ACCESS_KEY`\n\n### Azure Service Principal credentials\n\nThose AzureRM credentials are loaded only if you are using the Service Principal mode. They are acquired from the profile defined in `~/.azurerm/config.yml`\n\n- `ARM_CLIENT_ID`\n- `ARM_CLIENT_SECRET`\n\n### GCP configuration\n\nThose GCP related variables are available from the environment when using the example configuration:\n\n- `TF_VAR_gcp_region`\n- `TF_VAR_gcp_gcp_zone`\n- `TF_VAR_gcp_gcp_project`\n\n### GKE configurations\n\nEach GKE instance has its own kubeconfig, the path to each configuration is available from the environment:\n\n- `TF_VAR_gke_kubeconfig_${gke_cluster_name}`\n\nkubeconfig is automatically fetched by the wrapper (using gcloud) and stored inside the `.run` directory of your project.\nIt is refreshed automatically at every run to ensure you point to correct Kubernetes endpoint.\nYou can disable this behaviour by setting `refresh_kubeconfig: never` in your cluster settings.\n\n```yaml\n---\ngcp:\n  general:\n    mode: adc-user\n    project: &gcp_project project-name\n  gke:\n    - name: kubernetes-1\n      zone: europe-west1-c\n      refresh_kubeconfig: never\n```\n\n### Stack configurations and credentials\n\nThe `terraform[\'vars\']` dictionary from the stack configuration is accessible as Terraform variables.\n\nThe profile defined in the stack configuration is used to acquire credentials accessible from Terraform.\nThere is two supported providers, the variables which will be loaded depends on the used provider.\n\n- `TF_VAR_client_name`\n- `TF_VAR_aws_account`\n- `TF_VAR_aws_region`\n- `TF_VAR_aws_access_key`\n- `TF_VAR_aws_secret_key`\n- `TF_VAR_aws_token`\n- `TF_VAR_azurerm_region`\n- `TF_VAR_azure_region`\n- `TF_VAR_azure_subscription_id`\n- `TF_VAR_azure_tenant_id`\n- `TF_VAR_azure_state_access_key`\n\n### Stack path\n\nThe stack path is passed to Terraform. This is especially useful for resource naming and tagging.\n\n- `TF_VAR_account`\n- `TF_VAR_environment`\n- `TF_VAR_region`\n- `TF_VAR_stack`\n\n# Development\n\n## Tests\n\nAll new code contributions should come with unit and/or integrations tests.\n\nTo run those tests locally, use [tox](https://github.com/tox-dev/tox).\n\n## Debug command-line completion\n\nYou can get verbose debugging information for `argcomplete` by defining the following environment variable:\n\n```bash\nexport _ARC_DEBUG=1\n```\n\n## Python code formatting\n\nOur code is formatted with [black](https://github.com/psf/black/).\n\nMake sure to format all your code contributions with `black ${filename}`.\n\nHint: enable auto-format on save with `black` in your [favorite IDE](https://black.readthedocs.io/en/stable/editor_integration.html).\n\n## Checks\n\nTo run code and documentation style checks, run `tox -e lint`.\n\nIn addition to `black --check`, code is also checked with:\n\n- [flake8](https://gitlab.com/pycqa/flake8), a wrapper for [pycodestyle](https://github.com/PyCQA/pycodestyle) and [pyflakes](https://github.com/PyCQA/pyflakes).\n- [flake8-docstrings](https://gitlab.com/pycqa/flake8-docstrings), a wrapper for [pydocstyle](https://github.com/PyCQA/pydocstyle).\n\n## README TOC\n\nThis [README\'s table of content](#table-of-contents) is formatted with [md_toc](https://github.com/frnmst/md-toc).\n\nKeep in mind to update it with `md_toc --in-place github README.md`.\n\n## Using terraform development builds\n\nTo build and use development versions of terraform, manually put them in a `~/.terraform.d/versions/X.Y/X.Y.Z-dev/` folder:\n\n```bash\n# cd ~/go/src/github.com/hashicorp/terraform\n# make XC_ARCH=amd64 XC_OS=linux bin\n# ./bin/terraform version\nTerraform v0.12.9-dev\n# mkdir -p ~/.terraform.d/versions/0.12/0.12.9-dev\n# mv ./bin/terraform ~/.terraform.d/versions/0.12/0.12.9-dev/\n```\n\n## git pre-commit hooks\n\nSome git pre-commit hooks are configured in `.pre-commit-config.yaml` for use with the [pre-commit tool](https://pre-commit.com).\n\nUsing them helps avoiding to push changes that will fail the CI.\n\nThey can be installed locally with:\n\n```bash\n# pre-commit install\n```\n\nIf updating hooks configuration, run checks against all files to make sure everything is fine:\n\n```bash\n# pre-commit run --all-files --show-diff-on-failure\n```\n\nNote: the `pre-commit` tool itself can be installed with `pip` or `pipx`.\n\n## Tagging and publishing new releases to PyPI\n\nUse the `scripts/release.sh` script from `master` branch to:\n\n- bump the version with poetry,\n- update `CHANGELOG.md`,\n- commit these changes,\n- tag with last CHANGELOG.md item content as annotation,\n- bump the version with poetry again to mark it for development,\n- commit this change,\n- push all commits and tags to all remote repositories.\n\nThis will trigger a Github Actions job to publish packages to PyPI.\n\nTo invoke the script, pass it the desired bump rule, e.g.:\n\n```bash\n# ./scripts/release.sh minor\n```\n\nFor more options, check the help:\n\n```bash\n# ./scripts/release.sh --help\n```\n',
     'author': None,
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/claranet/terraform-wrapper',
```

### Comparing `claranet-tfwrapper-9.2.0/PKG-INFO` & `claranet-tfwrapper-9.2.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claranet-tfwrapper
-Version: 9.2.0
+Version: 9.2.1a0
 Summary: Claranet's `tfwrapper` is a wrapper for [Terraform](https://www.terraform.io/) implemented in python which aims to simplify Terraform usage and enforce best practices
 Home-page: https://github.com/claranet/terraform-wrapper
 License: Mozilla Public License Version 2.0
 Keywords: terraform,wrapper
 Requires-Python: >=3.6.2,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,24 +19,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Provides-Extra: azure
 Requires-Dist: CacheControl (>=0.12.6,<0.13.0)
 Requires-Dist: Jinja2 (>=3.0.1,<4.0.0)
-Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
+Requires-Dist: PyYAML (>=5.4.1,<7.0.0)
 Requires-Dist: argcomplete (<2.0)
 Requires-Dist: azure-cli-core (>=2.30.0,<3.0.0); extra == "azure"
 Requires-Dist: azure-common (>=1.1.27,<2.0.0); extra == "azure"
 Requires-Dist: azure-mgmt-storage (>=18.0.0,<19.0.0); extra == "azure"
 Requires-Dist: boto3 (>=1.17.94,<2.0.0)
-Requires-Dist: colorlog (>=5.0.1,<6.0.0)
+Requires-Dist: colorlog (>=5.0.1,<7.0.0)
 Requires-Dist: lockfile (>=0.12.2,<0.13.0)
 Requires-Dist: msrestazure (>=0.6.4,<0.7.0); extra == "azure"
-Requires-Dist: natsort (>=7.1.1,<8.0.0)
+Requires-Dist: natsort (>=7.1.1,<9.0.0)
 Requires-Dist: packaging (>=21.0,<22.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: schema (>=0.7.4,<0.8.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # claranet-tfwrapper
```

