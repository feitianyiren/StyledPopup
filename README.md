# StyledPopup
This plugin provides a standardized way to style view popups based on the user's color scheme.

The plugin will parse the users active color scheme and generate a style sheet which can be used to style the html displayed in the popup.

The classes generated are based on the scopes available within the color scheme. Since all color schemes are based on specific scopes, this provides a common method to style html elements.

## Usage

### HTML Markup

To style specific elements in the html, simply assign the element a class that matches the scope you would like to use.

<!-- language: lang-html -->

        <span class="keyword">This should be styled like a keyword</span>

Each nested scope selector should be applied as a seperate css class:

<!-- language: lang-html -->

        <span class="entity name class"> This should be styled similar to a support type within the color scheme</span>

![alt text](http://huotmedia.com/github/StyledPopup/images/screen_1.png)

### Calling the Styled Popup.

Import the module using:

<!-- language: lang-python -->

        from StyledPopup import styled_popup

Then call the styled_popup function passing the view associated with the popup and any arguments to be passed to the view's show_popup function.

## Future Tasks

1. Finalize code, clean-up, and commet
2. Implement styled code blocks with language based syntax coloring.
