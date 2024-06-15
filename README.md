## Get Started with Twitter Likes Visualization

Welcome to the future of Twitter likes visualization! Follow these steps to clone and run your very own Twitter likes visualization app. Now you too can see what your favorite people (like Elon Musk) are liking on Twitter, all from the comfort of your own command line. Let's dive in!

### Step 1: Clone the Repository

First, you need to clone the repository from GitHub. Think of it like SpaceX cloning the Falcon 9... but way easier and less expensive.

```bash
git clone https://github.com/clearclown/twitter_likes.git
cd twitter_likes
```

### Step 2: Prepare Your Environment

Create a `.env` file to store your secret keys. This is like your very own vault of secrets, but instead of housing Tesla’s autopilot code, it’s just your Twitter API keys.

Create a file named `.env` and add the following lines with your own keys:
### Retrieving New Tokens and Cookies

1. Log in to X (formerly Twitter) and open Developer Tools (F12 key).
2. Select the Network tab and monitor API requests.
3. From the request headers, obtain the latest `auth_token` and `ct0`.
4. Re-run the commands with the updated tokens and cookies.

Simple as that!
```env
BEARER_TOKEN=your_bearer_token
AUTH_TOKEN=your_auth_token
CT0=your_ct0_token
COOKIE='your_cookie_data'
```

Remember, with great power comes great responsibility. Don’t share your API keys!

### Step 3: Build the Docker Image

Next, let’s build the Docker image. It's like building a rocket, but instead of engineers and rocket fuel, you just need Docker.

```bash
docker build -t twitter-likes-app ./app
```

### Step 4: Run the Docker Container

Now, let's launch this bad boy! Start your Docker container, and watch it lift off just like the SpaceX Starship (minus the explosion, hopefully).

```bash
docker run --env-file .env -p 8000:8000 twitter-likes-app
```

### Step 5: Open Your Browser

Time to see the magic happen. Open your browser and go to:

[http://localhost:8000/](http://localhost:8000/)

You’ll be greeted with a sleek interface where you can enter a Twitter screen name. Hit the "Get Likes" button, and voilà! You’ll see what tweets Elon Musk (or any other user) has been liking.

### Step 6: Enjoy the Show

Sit back, relax, and enjoy the show. You can now visualize tweets liked by anyone (with public likes), including our favorite tech billionaire, Elon Musk. 

Remember, in a world where you can be anything, be kind. Or at least, don't be like Elon on Twitter.

### Troubleshooting

If something doesn't work as expected, just remember: it's not a bug, it's a feature! (Or, as Elon would say, "It's just a minor, rapid unscheduled disassembly.")

### Conclusion

There you have it! You’re now equipped to clone, run, and enjoy your very own Twitter likes visualization tool. Who knows, maybe your next step will be to develop an AI that writes tweets for you. Just remember, tweeting like Elon comes with its own set of responsibilities.

Happy coding!

---

Feel free to modify the guide according to your specific repository details and API keys. And remember, always tweet responsibly!
