# capacitor-secure-storage demo

This Ionic/Vue app demonstrates all of the features of the [capacitor-secure-storage plugin](https://github.com/aparajita/capacitor-secure-storage).

## Installation

First clone the repo locally:

```shell
git clone https://github.com/aparajita/capacitor-secure-storage-demo
```

Install dependencies:

```shell
pnpm install
npm install
yarn
```

Build:

```shell
pnpm build && cap sync
npm run build && cap sync
yarn build && cap sync
```

## Running

On the web:

```shell
pnpm serve
npm run serve
yarn serve
```

On iOS:

```shell
pnpm ios
npm run ios
yarn ios
```

On Android:

```shell
pnpm android
npm run android
yarn android
```

## Usage

**Set the prefix**<br>
To change the key prefix, edit the "Prefix" field and press "Set".

**View all keys**<br>
To view all of the keys in storage with the current prefix, press "Keys".

**Set a value**<br>
To set a value in storage, enter the key name in the "Key" field and a JSON-parseable value in the "Data" field. As you type in the "Data" field, if it is a valid value, the data type is displayed in parentheses after the "Data" label.

You may store any valid JSON value: string, number, boolean, array, object, or null. In addition, if the "Data" field looks like an ISO 8601 datetime (begins with YYYY-MM-DD), it is parsed as such, and if successfully parsed the type will be shown as "date". Note that the time and milliseconds are optional. So, for example, these are all parsed as a valid date:

```
2020-08-27
2020-08-27T13:27:07
2020-08-27T13:27:07.413Z
```

**Get a value**<br>
To get a value from storage, enter the key name and press "Get".

**Remove an item**<br>
To remove an item from storage, enter the key name and press "Rm".

**Clear all values**<br>
To remove all items from storage with the current prefix, press "Clear".
