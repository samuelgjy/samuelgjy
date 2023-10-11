### Hey there!! 👋
I'm Samuel, an aspiring professional in Applied Artificial Intelligence, currently advancing my knowledge at SIT. My insatiable curiosity and unwavering passion for innovation drive my journey in the captivating realms of Machine Learning and Data Science. I'm on a mission to unearth the transformative power these fields hold and how they can reshape our world. I'm always open to connect, collaborate, or simply have a chat. Feel free to reach out!"

import requests
import base64

# Replace with your GitHub username and repository
username = "samuelgjy"
repository = "samuelgjy"

# Make a request to get the README content
url = f"https://api.github.com/repos/{username}/{repository}/readme"
response = requests.get(url)

if response.status_code == 200:
    readme_data = response.json()
    readme_content = base64.b64decode(readme_data['content']).decode('utf-8')

    # Now, you can parse and analyze the `readme_content` to identify the most used languages.
    # Follow the steps mentioned earlier for this analysis.
else:
    print("Error: Unable to fetch README content.")
<!--
**samuelgjy/samuelgjy** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.
ads
Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
