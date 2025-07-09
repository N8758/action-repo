# 📦 action-repo

This is the GitHub repository that triggers webhook events.

When I push code or open a pull request in this repo, GitHub sends a webhook to my backend Flask server in the `webhook-repo`.

---

## 🔁 What This Repo Does

- ✅ Sends `push` events
- ✅ Sends `pull_request` events
- ✅ Used only to **generate activity** for testing and displaying in a live dashboard

---

## 🌐 Webhook Configuration

I have set a webhook in:

**Settings → Webhooks**  
With this configuration:

- ✅ Payload URL: `https://<ngrok-url>.ngrok-free.app/webhook`
- ✅ Content Type: `application/json`
- ✅ Events selected: `push`, `pull_request`

---

## 📦 Example

If I commit a file here (e.g. `test.txt`), this will:
- Trigger a `push` event
- GitHub will send it to my Flask server
- It gets stored in MongoDB
- It shows up live on my dashboard

---

## 🔗 Related Repo

👉 Main backend and dashboard:  
[webhook-repo](https://github.com/YOUR_USERNAME/webhook-repo)

---

## 🧑‍💻 Author

**Nilesh Pulate**
