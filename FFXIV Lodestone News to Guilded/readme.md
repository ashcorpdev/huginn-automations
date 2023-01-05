This scenario will grab the latest news posts from the Final Fantasy XIV Online website (via the Lodestone News API) and publish them to a Guilded Webhook.

# Setup

## Guilded
You will need to create a Webhook for the channel you want have the posts sent to in Guilded. To do this:

1. Click on the 'Settings' button for your chosen channel.
2. Click on the 'Webhooks' option on the left-hand sidebar.
3. Click on the 'Create a Webhook' button, and specify your preferred name and image for the Webhook.
4. Copy the URL and save it for later.

> Be aware that this URL should be considered **secret** - anyone with this URL can post to this channel, even if they are not in the server.

## Huginn
Once you have configured your Webhook in Guilded, do the following:

1. Go to 'Credentials' page via the navigation bar.
2. Click on the 'New Credential' button and put the following as the name: `guilded_lodestone_news_webhook_url`
3. In the section that says 'Credential Value', paste in the Webhook URL you got from Guilded earlier.
4. Click on the 'Save Credential' button.
5. Go to the 'Scenarios' page via the navigation bar.
6. Click on the 'Import Scenario' button.
7. Either paste the link of the raw json file from GitHub, or download a copy of the scenario `.json` file and upload it here.

> GitHub URL: https://raw.githubusercontent.com/ashcorpdev/huginn-automations/main/FFXIV%20Lodestone%20News%20to%20Guilded/ffxiv-lodestone-news-to-guilded.json

8. Click on the 'Start Import' button and you should be prompted with a screen showing you what agents will be created as part of the import.
9. Check the box that says 'I confirm that I want to import these Agents.' and then click the 'Finish Import' button.
10. You should now see the scenario and a popup saying 'Import Successful'.
