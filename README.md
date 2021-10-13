- 👋 Hi, I’m @75797579pat
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
75797579pat/75797579pat is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->// Dapps
https://registry.walletconnect.org/data/dapps.json

// Wallets
https://registry.walletconnect.org/data/wallets.json

// Logos
// [size] = "sm" | "md" | "lg"
// [id] = present in app entry
https://registry.walletconnect.org/logo/[size]/[id].jpeg
interface AppEntry {
  id: string;
  name: string;
  homepage: string;
  chains: string[];
  app: {
    browser: string;
    ios: string;
    android: string;
    mac: string;
    windows: string;
    linux: string;
  };
  mobile: {
    native: string;
    universal: string;
  };
  desktop: {
    native: string;
    universal: string;
  };
  metadata: {
    shortName: string;
    colors: {
      primary: string;
      secondary: string;
    };
  };
}

interface AppRegistry {
  [id: string]: AppEntry;
}
