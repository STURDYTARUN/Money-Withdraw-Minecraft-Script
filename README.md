# 💸 Money Note Skript (Withdraw & Redeem System)

A fully functional **Minecraft Skript** that lets players convert their in-game money into physical items (Money Notes) and redeem them anytime. Perfect for economy-based servers, trading systems, and roleplay setups.

---

## 📖 Overview

This skript introduces a **withdraw system** where players can turn their balance into a tradable paper item. Each note stores its value in the lore and can be redeemed simply by right-clicking it.

This allows:

* Safe player-to-player trading 💰
* Physical representation of money 📜
* Easy transfers without commands 🤝

---

## ✨ Features

* 🏦 `/withdraw <amount>` command
* 📜 Custom paper item with name & lore
* 🔢 Unique hidden ID for each note
* 🖱️ Right-click to redeem money
* 🚫 Prevents invalid amounts (negative/zero)
* ❌ Stops usage if player has insufficient balance
* ⚡ Lightweight & efficient (no lag impact)

---

## ⚙️ Requirements

Make sure your server has:

* **Skript plugin**
* **Vault** (for economy support)
* Any Vault-supported economy plugin (like EssentialsX Economy)

---

## 📥 Installation

1. Install required plugins (Skript + Vault + Economy)
2. Download this skript file
3. Place it in:

   ```
   /plugins/Skript/scripts/
   ```
4. Reload Skript:

   ```
   /skript reload all
   ```
5. You're good to go ✅

---

## 🚀 Usage

### Withdraw Money

```
/withdraw <amount>
```

* Converts your balance into a **Money Note**
* Example:

  ```
  /withdraw 500
  ```

  → You receive a paper worth ₹500

---

### Redeem Money

* Right-click the **Money Note**
* The stored value is added back to your balance

---

## 🧩 How It Works

* When a player withdraws money:

  * Amount is removed from their balance
  * A paper item is created
  * Value is stored in the item's lore
  * A random ID is added (for uniqueness)

* When redeeming:

  * Skript reads the lore
  * Extracts the value
  * Adds money back to the player
  * Removes the note

---

## 📜 Example Item

**Name:**

```
Money Note (₹500)
```

**Lore:**

```
Right-click to redeem  
Value: 500  
ID: 123456
```

---

## ⚠️ Notes

* Do NOT manually edit the item lore, or it may break
* Value is parsed from lore, so formatting matters
* Works only with paper items named "Money Note"

---

## 🔮 Future Ideas (Optional Improvements)

* Anti-duplication system
* Database tracking for notes
* Custom textures for notes
* Expiry system for notes
* Support for multiple currencies

---

## 🤝 Contributing

Feel free to fork, improve, or suggest features. Pull requests are welcome!

---

## 📄 License

Free to use and modify for personal or public servers.

---

## ❤️ Support

If you found this useful, consider giving the repo a ⭐
