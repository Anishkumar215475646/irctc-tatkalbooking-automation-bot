# This is just my experimental project because i am facing so much difficulty in booking tatkal ticket.



## 🚂 IRCTC Tatkal Cypress Automation (Apna Jugaad)

### Ab 1 minute ke andar tatkal tickets book karo! Isme captcha automatic bypass hoga aur ek saath multiple passengers ki details khud-ba-khud fill ho jayengi. Tujhe bas script chalu karke aaram se baithna hai.

🙏😍👏🙏😍🙏👏🙏😍🙏👏🙏😍🙏😍🙏👏🔥👍🔥👍🔥👍🔥

> ⚠️ **IMPORTANT NOTE (Padh lo pehle):** > Yeh Cypress script sirf educational purposes aur seekhne ke liye banayi gayi hai.
> IRCTC ke terms aur rules mat todna. Agar koi legal lafda hota hai,
> toh uske zimmedar tum khud hoge, author nahi! Baki tu samajhdar hai.

---

## 🚀 Mast Features Kya-Kya Hain?

-  ✓ **Tatkal**, **Premium Tatkal** aur **Normal Tickets** sab book kar sakta hai.
-  ✓ Agar Tatkal time se **2-3 minute pehle** bhi script chalu karega, toh ye sahi time ka wait karegi aur automatic shuru ho jayegi.
-  ✓ **Username** aur **password** se auto login.
-  ✓ **Auto Upgradation** aur "Book only if confirm berths are allotted" automatic tick ho jata hai.
-  ✓ **Multiple passengers** ka full support hai (sabka data ek sath bharega).
-  ✓ **Food Choices** aur **Seats Preferences** ka option hai.
-  ✓ **Payment Gateway Automation:** Direct UPI ID par request phekega ya fir screen par QR Code dikha dega, bas scan karo aur pay karo!

---

## 🛠️ Isko Apne System Pe Kaise Setup Karein?

Sabspe pehle tere computer me **NodeJS** aur **Python** installed hona chahiye.

### 1. Passenger Ka Data Bharna (`cypress/fixtures/passenger_data.json`)
Is file me jaakar apni train aur passenger ki details change kar le.

> 💡 **Tip:** Agar `UPI_ID_CONFIG` me apni UPI ID dalega, toh seedhe tere phone par payment request aayegi (2-3 seconds lagte hain aane me). Agar isko khali chhodega, toh script QR Code wale page par ruk jayegi, wahan scan karke turant pay kar dena, wo jyada fast hota hai!

> ⚠️ **Note:** Ek baar me ya toh `TATKAL` true hoga ya `PREMIUM_TATKAL`, dono ko ek sath true mat karna!

**Example JSON format:**
```json
{
  "TRAIN_NO": "12318",
  "TRAIN_COACH": "3A",
  "TRAVEL_DATE": "12/09/2026",
  "SOURCE_STATION": "UMB",
  "BOARDING_STATION": null,
  "DESTINATION_STATION": "BSB",
  "TATKAL": true,
  "PREMIUM_TATKAL": false,
  "UPI_ID_CONFIG": "yourupi@paytm",
  "PASSENGER_DETAILS": [
    {
      "NAME": "ANISH VERMA",
      "AGE": 25,
      "GENDER": "Male",
      "SEAT": "Side Upper",
      "FOOD": "No Food"
    }
  ]
}
