# Yankp - Copy File or Directory Paths to Clipboard

`yankp` is a simple yet handy shell tool that lets you **copy the current working directory** or the **absolute path to a specific file** into your **system clipboard** using `xclip` (Linux) or `pbcopy` (macOS).  

Perfect for terminal lovers, script writers, bug bounty hunters, and anyone tired of typing out long paths!

---

## ✨ Features

- 📁 Copy current working directory to clipboard  
- 📄 Copy full file path of any file under the current directory  
- 🔍 Auto-detect and install clipboard utilities (`xclip`, `pbcopy`)  
- 🧼 Minimal, dependency-light, pure Bash  
- 📖 Built-in help menu via `yankp -h`

---

## ⚙️ Installation

You have two ways to install `yankp`:

### 🧰 Option 1: Manual Installation

```bash
git clone https://github.com/yourusername/yankp.git
cd yankp
chmod +x yankp
sudo mv yankp /usr/local/bin/

📦 Option 2: Install via APT (Debian/Ubuntu-based systems)

echo "deb [trusted=yes] https://sarojamkatel.github.io/yankp-deb/repo ./" | sudo tee /etc/apt/sources.list.d/yankp.list
sudo apt update
sudo apt install yankp