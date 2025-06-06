# LuaAssembly Capture-the-flag challenge

This project is licensed under [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/).  
This is the first LASM runtime in Luau released with bytecode that contains a CTF challenge.

## ❓ What is LuaAssembly

LuaAssembly is a new way of integrating security-critical code into your Lua environments. You can find more information upon the release of our developer tools.

## 🚀 CTF

Inside the script, you will find a variable called `INPUT_STRING`. This string will be encrypted by the runtime module and then printed out in a string and bytes form. Your goal is to reverse the encryption algorithm and decrypt the encrypted flag, which was also encrypted using the same script.

## 🏎️ Running the CTF

You can run the CTF by executing the command `luau ctf.luau`. Luau has to be installed for that.

## 💪 Difficulty

This CTF does not contain any "obfuscated" code, but it contains a virtual-machine which interprets bytecode and acts in a special way. It may be harder to reverse or keep track of, but should definitely be manageable to solve.

## 🚩 Encrypted Flag (bytes)

```js
[
    0x9b, 0x3c, 0xd8, 0x5c, 0xf5, 0xf3, 0xe9, 0x0, 0xd6, 0xdc, 0xbb, 0x19, 0xdf,
    0x60, 0xf4, 0x78, 0xf1, 0xe7, 0x5, 0xf4, 0xe2, 0x8, 0xff, 0x67, 0x71, 0x2,
    0x20, 0xe, 0xe5, 0x1b, 0x87, 0x7a, 0x70, 0x82, 0xd3, 0xe9, 0xef, 0xfe, 0x34,
    0x80, 0x8b, 0x1f, 0xf5, 0x76, 0x7c, 0x76, 0x69, 0x3d, 0xfb, 0xea, 0x8a, 0x6,
    0x15, 0x95, 0x77, 0x18, 0x2e, 0x1c, 0x33, 0x29, 0x8d, 0xee, 0x1c, 0x12,
    0x31, 0x27, 0xcb, 0x96, 0xbc, 0x8e, 0xf, 0xa7, 0x89, 0x42, 0x20, 0x3e, 0x87,
    0xb5, 0x29, 0x20, 0x4e, 0xba, 0xa5, 0xcb, 0xa5, 0x36, 0xae, 0xd8, 0x9b,
    0xc9, 0x25, 0xbe, 0x2a, 0xce, 0xa9, 0x25, 0xd9, 0x9c, 0x70, 0xec, 0xbf,
    0x33, 0xa7, 0x58, 0x76, 0xea, 0xc5, 0x41, 0xcd, 0x4e, 0xde, 0xf8, 0x41,
    0xe1, 0x5d, 0x24, 0x42, 0xe6, 0xd1, 0xd7, 0xf9, 0x6a, 0x68, 0x6e, 0x55,
    0x8b, 0xff, 0x38, 0x7e, 0x2c,
];
```

The unencrypted flag has the following format: `{ HEX }`.

## 📰 Notice

This sample is just a minimal working example of the LuaAssembly project. When our project is working, we will open-source runtimes and other developer tools that were also used to create this sample. Thank you for participating. If you're someone who found this repository and solved the challenge, congratulations! We don't have any special prize, but you could create an Issue on this repository to get into contact.
