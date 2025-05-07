### Option 1
If you want to view the key manually, you can read it using PowerShell:
1. Open PowerShell as an administrator.
2. Enter the following command:
```powershell
(Get-WmiObject -query 'select * from SoftwareLicensingService').OA3xOriginalProductKey
```

With that PS command you can see the saved OEM-Key from youre BIOS.

If you want to re register it for youre windows computer do this:
1. Open CMD as an administrator.
2. Enter the following command:
```batch
slmgr.vbs /ipk YOURE-PRODUCT-KEY
slmgr.vbs /ato
```
