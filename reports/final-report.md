# Phishing Email Analysis Report

## Project

Phishing Email Analysis and Prevention

## Objective

Analyze a phishing email and identify phishing indicators.

---

## Email Information

**Sender:** support@secure-bank-login.com

**Subject:** Urgent! Verify Your Bank Account

---

## WHOIS Analysis

### Command

```bash
whois secure-bank-login.com
```

### Result

No match for domain "SECURE-BANK-LOGIN.COM"

### Observation

- Domain is not registered.
- Sender is not associated with a legitimate organization.
- This is a strong indicator of a phishing attempt.

---

## DNS Analysis

### Command

```bash
host secure-bank-login-update.com
```

### Output

```
Host secure-bank-login-update.com not found: 3(NXDOMAIN)
```

### Observation

- The domain could not be resolved.
- DNS returned an NXDOMAIN response.
- The domain does not appear to be registered or active.
- This increases suspicion that the email is fraudulent.

---

## URL Analysis

### URL

http://secure-bank-login-update.com/login

### Findings

- Uses HTTP instead of HTTPS.
- Contains suspicious keywords:
  - login
  - secure
  - update
  - bank
- Attempts to imitate a banking website.
- The URL may be used to steal user credentials.

### Risk

High

---

## VirusTotal Analysis

### Tool Used

VirusTotal

### URL

http://secure-bank-login-update.com/login

### Results

- Detection Score: 0/95
- Most security vendors reported the URL as Clean.
- Last Analysis: 4 months ago.

### Observation

Although VirusTotal did not detect the URL as malicious, it still contains several phishing indicators:

- Uses HTTP instead of HTTPS.
- Contains suspicious keywords (secure, bank, login, update).
- The associated domain could not be verified through WHOIS and DNS analysis.

---

### Conclusion

VirusTotal results alone should not be used to determine whether a URL is safe. The URL should still be treated as suspicious because of the phishing characteristics identified during analysis.
## Email Content Analysis

### Indicators Found

- Generic greeting ("Dear Customer")
- Urgent language
- Threatening message
- Unknown sender
- Suspicious URL
- HTTP instead of HTTPS

### Risk Level

**High**

---

## Recommendations

- Never click suspicious links.
- Verify the sender before responding.
- Enable Multi-Factor Authentication (MFA).
- Use email filtering.
- Train employees to identify phishing emails.
- Report suspicious emails immediately.

---

## Conclusion

The email contains multiple phishing indicators and should be treated as malicious.
