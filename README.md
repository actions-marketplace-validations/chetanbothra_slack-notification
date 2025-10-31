# 🚀 Slack Deployment Notification GitHub Action

This GitHub Action sends **deployment success / failure notifications** to Slack with rich formatting, commit info, and links — perfect for DevOps CI/CD pipelines.

---

## ✨ Features

- 🔔 Sends Slack alerts on deployment success & failure
- 🧠 Reads GitHub deployment event data automatically
- 🎨 Beautiful Slack Block UI
- 👤 Shows commit author & message
- 🔗 Links to GitHub Workflow run
- 🔒 Uses secure Slack Bot Token

---

## 📦 Usage

Add this step to your deployment workflow:

```yaml
- name: Slack Deploy Notification
  uses: chetanbothra/slack-deploy-action@v1
  if: always()
  with:
    slack_token: ${{ secrets.SLACK_BOT_TOKEN }}
    slack_channel: "#deployments"
