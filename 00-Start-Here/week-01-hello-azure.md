# Week 01 — Hello Azure (Azure CLI Proof)

## Goal

Prove I can authenticate and manage Azure resources using the Azure CLI.

---

## 1) Azure CLI Installed

**Command:**

```bash
az version
```

- azure-cli: "2.83.0"
  [Azure Version](/00-Start-Here/Images/az-version.png)

## 2) Login

```bash
az login
```

**Result**

- Login completed successfully
  [Login Completed](/00-Start-Here/Images/login-successful.png)

## 3) Confirm Account/Subscription

```bash
az account show
```

**Result**

- Subscription Name: "Testing"
  [Account Show](/00-Start-Here/Images/az-account-show.png)

```bash
az account list --output table
```

[AZ Account List](/00-Start-Here/Images/account-list-table.png)

## 4) Create Resource Group

```bash
az group create --name rg-week01-hello-azure --location eastus
```

**Result:**

- provisioningState:Succeeded
  [Resource Group Created](/00-Start-Here/Images/resource-group-created.png)

## 5) List Resource Group

```bash
az group list --output table
```

**Result**

- I can see rg-week01-hello-azure in the table output.
  [Resource Group Table](/00-Start-Here/Images/resource-group-table.png)

## 6) Delete Resource Group

**Command**

```bash
az group delete --name rg-week01-hello-azure --yes --no-wait
```

**Confirm deletion Command:**

```bash
az group exists --name rg-week01-hello-azure
```

**Result**

- false
  [False Result](/00-Start-Here/Images/false-result.png)
