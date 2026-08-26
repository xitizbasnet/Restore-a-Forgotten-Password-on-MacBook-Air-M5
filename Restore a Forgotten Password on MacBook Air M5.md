#  Restore a Forgotten Password on MacBook Air M5

## 📘 Overview

This lab explains how to restore access to a MacBook Air M5 when the login password has been forgotten.

The primary challenge when resetting a Mac password is **FileVault**. When enabled, FileVault encrypts the SSD and prevents unauthorized access to data stored on the device.

To reset the password successfully, you typically need one of the following:

- The Mac account password
- The FileVault Recovery Key
- Access to the Apple Account associated with the Mac

If the recovery key is unavailable, another Apple device signed in to the same Apple Account may help retrieve it.

> **Important**
>
> If FileVault is enabled and neither the password nor recovery key is available, access to the encrypted data may not be possible.

---

## 🔐 Part A: Access macOS Recovery

### Step 1: Power Off the MacBook

If you cannot sign in to macOS:

1. Press and hold the **Power** button until the screen turns off.
2. Wait a few seconds.
3. Press and hold the **Power** button again.
4. Continue holding when you see:

```text
Continue holding for startup options
```

5. Release the Power button when the message changes to:

```text
Loading startup options
```

---

### Step 2: Open Startup Options

1. Select **Options**.
2. Click **Continue**.
3. Wait for macOS Recovery to load.

---

## 🔑 Part B: Recover Access Using an Apple Account

### Step 3: Select "Forgot All Passwords"

If you do not know the password for any local user account:

1. Select **Forgot All Passwords**.
2. Proceed to connect the MacBook to Wi-Fi.

---

### Step 4: Connect to Wi-Fi

1. Click the **Wi-Fi** icon at the top-right corner.
2. Select the wireless network.
3. Enter the Wi-Fi password.
4. Press **Enter**.

✅ Internet connectivity is required to continue the recovery process.

---

### Step 5: Sign In to the Apple Account

Sign in using the Apple Account linked to the MacBook.

> **Note**
>
> This is your **Apple Account**, not your macOS user account.

1. Enter the Apple Account email address.
2. Press **Enter**.
3. Enter the password.
4. Click **Next**.
5. Wait for authentication to complete.

After successful sign-in, the recovery options become available.

> **Note**
>
> Depending on the macOS version, the recovery screen may appear automatically without requiring all previous steps.

---

## ⚙️ Part C: Reset the MacBook Password

### Step 6: Open Terminal

From the Recovery menu:

1. Select **Utilities**.
2. Select **Terminal**.

---

### Step 7: Run the Password Reset Command

In Terminal, enter:

```text
resetpassword
```

Press **Enter**.

> **Note**
>
> The standard macOS password-reset utility command is:
>
> ```text
> resetpassword
> ```
>
> This launches the Password Reset Assistant.

---

### Step 8: Select "I Forgot My Password"

1. Select **I Forgot My Password**.
2. Click **Next**.

You will be prompted to provide the FileVault Recovery Key.

---

## 🔐 Part D: Retrieve the FileVault Recovery Key

### Step 9: Enter the Recovery Key

If you have previously saved the FileVault Recovery Key:

1. Enter the recovery key.
2. Continue to the next step.

If the recovery key is unavailable, check another Apple device signed in to the same Apple Account.

---

### Step 10: Open the Passwords Application

On another Apple device signed in with the same Apple Account:

1. Open the **Passwords** application.
2. Authenticate if prompted.
3. Use the search option.
4. Search for the MacBook name.

Examples:

```text
MacBook
```

```text
Xitiz's MacBook Air
```

---

### Step 11: Locate the Recovery Key

Open the MacBook entry displayed in the search results.

Example:

```text
ABC's MacBook Air
```

If available:

1. Copy the Recovery Key.
2. Return to the MacBook.
3. Paste the Recovery Key into the recovery field.
4. Press **Enter**.

✅ Access to the password reset process should now be available.

> **💡 Tip**
>
> Keep a secure copy of the FileVault Recovery Key in an approved password manager or enterprise password vault.

---

## 🔄 Part E: Create a New Password

### Step 12: Select the User Account

1. Choose the user account whose password needs to be reset.
2. Click **Next**.

---

### Step 13: Create a New Password

1. Enter the new password.
2. Confirm the password.
3. Enter a password hint.
4. Click **Next**.

✅ The password is now reset.

> **Best Practice**
>
> Use a strong password containing:
>
> - Uppercase letters
> - Lowercase letters
> - Numbers
> - Special characters

---

## 🚨 Part F: Erase the Mac if the Recovery Key Cannot Be Found

### Step 14: Use Recovery Assistant

If neither the password nor the FileVault Recovery Key can be recovered:

1. Open **Recovery Assistant**.
2. Select:

```text
Erase Mac
```

3. Follow the prompts.

The Mac will be erased and returned to its initial setup state.

> **⚠️ Warning**
>
> Selecting **Erase Mac** permanently removes all data stored on the device.
>
> Proceed only if password recovery is not possible.

---

## 🚀 Part G: Restart the MacBook

### Step 15: Restart the Device

After successfully resetting the password:

1. Close all open windows.
2. Click **Restart**.
3. Wait for macOS to boot normally.
4. Enter the new password.

✅ You should now be able to sign in successfully.

---

## 📝 Notes

> **Note**
>
> FileVault encrypts the SSD and prevents unauthorized access to data stored on the Mac.

> **Note**
>
> Access to another Apple device signed in to the same Apple Account may help retrieve the FileVault Recovery Key.

> **Note**
>
> Some macOS versions may display recovery options automatically without requiring all recovery steps outlined above.

---

## 🔧 Troubleshooting

### Password Reset Utility Does Not Open

Verify the command entered in Terminal:

```text
resetpassword
```

Ensure there are no spaces in the command.

---

### Unable to Sign In to Apple Account

Verify:

- Internet connectivity
- Apple Account credentials
- Multi-Factor Authentication approval
- Apple service availability

---

### Recovery Key Cannot Be Found

Check:

- Passwords application on other Apple devices
- Enterprise password vaults
- Documentation provided during Mac enrollment
- IT Asset Records

If unavailable, proceed with:

```text
Recovery Assistant → Erase Mac
```

---

## 💡 Best Practice Tips

- Store the FileVault Recovery Key securely after device deployment.
- Link the MacBook to an Apple Account before enabling FileVault.
- Maintain backup copies of important files using approved backup solutions.
- Keep at least one additional trusted Apple device signed in to the same Apple Account.
- Document asset information, recovery details, and ownership records for corporate devices.

---

 
