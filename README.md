# URL Shortening: Free and Unlimited URL Shortening with Power Automate

This project provides a solution for shortening long SharePoint URLs or other URLs using Microsoft Power Automate. Create unlimited shortened URLs and use custom domain redirects effortlessly. If you need help setting this up on your own server, please contact me at huseyin_korhan@zetaleap.com.

## How It Works

1. Create a Folder in SharePoint:
- First, create a folder named "shorten_url" under the "Documents" section in SharePoint.

2. Create a Power Automate Flow:
- Log in to Power Automate and create a new flow.

3. Set Up the Trigger:
- Select the SharePoint trigger "When a file is created (properties only)" and choose the folder path you just created.

4. Add HTTP Action:
- Add an HTTP action and configure it according to the settings provided on the screen.
  - Method: POST
  - URI: https://zetaleap.com/shorten/
  - Use the following JSON for the body:
```json
{
  "target_url": "your_url",
  "api_key": "(Obtain your activation code from zetaleap.com)"
}
```
  

5. Update File Properties:
- Use the "Update file properties" action to save the newly created shortened link back to SharePoint.

![image-4](https://github.com/korhanh/PowerAutomate_Image_to_PDF/blob/main/4.png)


## Features

- Unlimited Shortening: Create as many shortened URLs as needed without any restrictions.
- Custom Domain Redirects: Use your own domain for URL redirects.
- Easy Setup: Follow the step-by-step guide to configure and customize the flow according to your needs.

## Requirements

- Microsoft Power Automate subscription
- Basic knowledge of SharePoint and Power Automate flow creation

## Getting Started

- Follow the steps outlined above to add the necessary actions to your Power Automate flow.
- Customize the folder paths and settings as needed.

  ## Contributions and Feedback

Contributions to this project are welcome! If you encounter any issues or have suggestions for improvement, feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](https://github.com/korhanh/PowerAutomate_Image_to_PDF/blob/main/LICENSE).

Feel free to use, modify, and distribute this project according to the terms specified in the license.

## Credits

This project is created and maintained by [korhanh]([link_to_your_github_profile](https://github.com/korhanh)).

If you use this project or find it helpful, consider giving it a star on GitHub!

