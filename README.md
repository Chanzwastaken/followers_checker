# Instagram Followers Checker

This Python script compares your Instagram followers with the people you're following to find out who isn't following you back. The script uses Instagram data exported in JSON format to perform this comparison.

## How it Works

- The script reads two JSON files: one containing your followers and another containing the accounts you are following.
- It then compares the two lists and outputs a list of accounts that you are following but who do not follow you back.

## Files

- `f_checker.py`: The main script to compare the follower and following data.
- `data/`: Folder containing Instagram data files.
  - `followers_1.json`: Contains a list of users who follow you.
  - `following.json`: Contains a list of users you follow.

## How to Get Your Instagram Follower and Following Data

1. **Request Your Instagram Data:**
   - Go to the [Instagram website](https://www.instagram.com/) and log in.
   - Go to your profile, click on the **Settings** gear icon, and select **Privacy and Security**.
   - Scroll down to **Data Download** and click **Request Download**.
   - Instagram will email you a link to download your data.

2. **Download the JSON Data:**
   - Download the data from the link sent to your email.
   - Extract the ZIP file, and inside, locate the `followers_1.json` file under the `followers_and_following` folder for your followers and `following.json` for the accounts you follow.

3. **Place the Files in the `data/` Folder:**
   - Place `followers_1.json` and `following.json` in the `data/` folder of the repository.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/Chanzwastaken/followers_checker.git
   cd followers_checker
   ```

2. Ensure you have Python installed on your machine.

3. Install necessary libraries (if needed):
   ```bash
   pip install json
   ```

4. Run the script:
   ```bash
   python f_checker.py
   ```

5. The script will output a list of users who do not follow you back in the following format:
   ```
   https://www.instagram.com/username
   ```

## Contributing

Feel free to fork this repository and make improvements! If you'd like to suggest a feature or report a bug, please open an issue.

## License

This project is licensed under the MIT License.
