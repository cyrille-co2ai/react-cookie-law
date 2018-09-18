# React Cookie Law

A React Cookie Banner component GDPR compliance.

## Install

```
yarn add @palmabit/react-cookie-law
```

or

```
npm install --save @palmabit/react-cookie-law
```

## Usage

```js
import CookieBanner from 'react-cookie-law';

React.renderComponent(
  <div>
    <CookieBanner
      message="Cookie banner messate"
      onAccept = {() => {}}
      onAcceptPreferences = {() => {}}
      onAcceptStatistics = {() => {}}
      onAcceptMarketing = {() => {}}
    />
  </div>,
  document.body
);
```

### Options

|Name|Type|Default|Description|
|----|----|-------|-----------|
| **message** | string | | **Required**. Custom text of the banner |
| **policyLink** | string | "/#" | *optional*. Link to privacy policy page |
| **privacyPolicyLinkText** | string | "Privacy Policy" | *optional*. Text for the privacy policy link |
| **necessaryOptionText** | string | "Necessary" | *optional*. Text for the *necessary* cookies checkbox |
| **preferencesOptionText** | string | "Preferences" | *optional*. Text for the *preferences* cookies checkbox |
| **statisticsOptionText** | string | "Statistics" | *optional*. Text for the *statistics* cookies checkbox |
| **marketingOptionText** | string | "Marketing" | *optional*. Text for the *marketing* cookies checkbox |
| **acceptButtonText** | string | "Accept" | *optional*. Text for the *accept* button |
| **declineButtonText** | string | "Decline" | *optional*. Text for the *decline* button |
| **showDeclineButton** | bool | false | *optional*. Show or hide the *decline* button |
| **dismissOnScroll** | bool | false | *optional*. Enable or disable the dismissing on scroll of the banner |
| **showPreferencesOption** | bool | true | *optional*. Show or hide the *preferences* checkbox |
| **showStatisticsOption** | bool | true | *optional*. Show or hide the *statistics* checkbox |
| **showMarketingOption** | bool | true | *optional*. Show or hide the *marketing* checkbox |
| **onAccept** | function | Function | *optional*. Callback called when the consent is given |
| **onAcceptPreferences** | function | Function | *optional*. Callback called if *preferences* cookies is accepted |
| **onAcceptStatistics** | function | Function | *optional*. Callback called if *statistics* cookies is accepted |
| **onAcceptMarketing** | function | Function | *optional*. Callback called if *marketing* cookies is accepted |
| **onDeclinePreferences** | function | Function | *optional*. Callback called if *preferences* cookies is declined |
| **onDeclineStatistics** | function | Function | *optional*. Callback called if *statistics* cookies is declined |
| **onDeclineMarketing** | function | Function | *optional*. Callback called if *marketing* cookies is declined |

## Style

```js
<CookieBanner
  message="Cookie banner messate"
  styles={{
    dialog: { backgroundColor: 'red' }
  }}
/>
```

|Style option|Description|
|----|----|
| **dialog** | Style that override `.react-cookie-law-dialog` class |
| **container** | `.react-cookie-law-container` class |
| **message** | Style for banner text (`.react-cookie-law-message` class) |
| **policy** | Style for cookie policy link (`.react-cookie-law-policy` class) |
| **selectPane** | Style for select pane (`.react-cookie-law-select-pane` class) |
| **optionWrapper** | Style for option checkbox wrapper (`.react-cookie-law-option-wrapper` class) |
| **optionLabel** | Style for the text of checkbox labels |
| **checkbox** | Style for checkboxes (`.react-cookie-law-option-checkbox` class) |
| **buttonWrapper** | Style for buttons wrapper (`.react-cookie-law-dialog` class) |
| **button** | Style for buttons (`.react-cookie-law-dialog` class) |

## Test

```
yarn test
```

or

```
npm test
```

# Author

[Palmabit](https://www.palmabit.com)

# Licence

[See the MIT License](http://opensource.org/licenses/MIT)