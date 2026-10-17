# 🎂 Birthday Friendship Slides

Ek chhota sa birthday surprise slideshow. Photos, videos, quotes aur ek personal note, sab background song ke saath. Poora project ek hi file mein hai: `index.html`.

## Features

- **Ek hi file:** photos, videos aur song sab file ke andar embedded hain. Alag se kuch download nahi karna padta.
- **Mobile-friendly:** phone par tap, swipe aur arrow buttons se chalta hai. Laptop par keyboard ke arrow keys aur Space bhi kaam karte hain.
- **Song control:**
  - "Surprise kholo" dabate hi pehli slide khulti hai aur song shuru ho jaata hai.
  - Last (END) slide aate hi song fade-out hokar band ho jaata hai.
  - "Phir se dekho" dabane par slideshow aur song dono dobara shuru se chalte hain.
  - Kabhi bhi 🔊 button se mute/unmute kar sakte ho.
- **Loading button:** page aur song load hone tak button "Surprise ban raha hai… 🎁" dikhata hai aur disabled rehta hai.
- **Auto mode:** upar left ke "▶ Auto" button se slides apne aap badalti hain (photo 5.5 sec, quote 7 sec, video 8 sec, aakhri note 11 sec). Dobara dabane par pause.
- **Fullscreen** button (jahan browser support kare).
- **WhatsApp preview:** link bhejne par title aur `og.jpg` ka birthday card dikhta hai.
- **"Thank you bolo 💌"** button END slide par, jo WhatsApp mein pehle se likha message khol deta hai.
- **Tab chhupe toh song pause** ho jaata hai aur wapas aane par resume.
- **Navigation:**
  - Screen ke right side par tap karo ya right swipe karo: agli slide.
  - Left 30% par tap karo ya left swipe karo: pichhli slide.

## Share kaise karein (WhatsApp ke liye link)

File ko seedha WhatsApp par bhejne se wo phone par aksar khulti nahi. Isliye pehle ise online host karo aur uska link bhejo.

1. File ka naam `index.html` rakho. Naam yahi hona zaroori hai.
   Saath mein `og.jpg` bhi usi folder mein upload karna, wahi WhatsApp ke link preview mein dikhti hai.
2. Neeche diye gaye options mein se koi ek chuno.

### Option 1: Netlify Drop (sabse aasaan)

1. Ek naya folder banao aur usmein `index.html` rakho.
2. Browser mein `app.netlify.com/drop` kholo.
3. Folder drag-drop karo.
4. Turant `something.netlify.app` jaisa link mil jayega.
5. Account bana kar site ko claim kar lo, taaki link expire na ho.

Chaaho toh site ka naam `neetu-birthday` jaisa kuch rakh sakte ho.

### Option 2: GitHub Pages (permanent, free)

1. github.com par free account banao.
2. Naya repository banao (jaise `birthday`).
3. "Add file → Upload files" mein `index.html` upload karo aur commit karo.
4. Settings → Pages mein "Deploy from a branch" chuno, branch `main` aur folder `/ (root)` select karke save karo.
5. 1 se 2 minute mein link ban jayega: `https://tumhara-username.github.io/birthday/`

GitHub Pages mein repository public hota hai, toh jiske paas link ho wo photos dekh sakta hai. Agar ye theek na lage toh Netlify use karo.

## Bhejne se pehle check kar lo

- Link kisi aur phone par khol kar dekho.
- "Surprise kholo" dabane ke baad song chalna chahiye. Phone silent mode mein ho toh iPhone par song nahi sunai deta, toh Neetu ko pehle bata dena.
- Sab photos aur videos load ho rahe hain ya nahi, ye poora ek baar chala kar dekh lo.
- END slide par song band hona chahiye.

## Settings badalna

`index.html` mein script ke shuru mein `WA_NUMBER` aur `WA_MSG` hain.

- `WA_NUMBER` mein apna number country code ke saath likho (jaise `919876543210`, bina + ya space ke). Tab "Thank you bolo" seedha tumhari chat khologa. Khali chhodoge toh Neetu ko contact chunna padega.
- `WA_MSG` mein wo message likho jo chat mein pehle se bhara aaye.

`og:image` ka link `https://surprise-psi-blush.vercel.app/og.jpg` hai. Agar Vercel project ka naam ya domain badlo toh `index.html` mein `og:image`, `twitter:image` aur `og:url` wali lines mein naya link daal dena.

## Text kaise badlein

Photos, videos aur song file ke andar encoded hain, isliye unhe badalna mushkil hai. Text badalna aasaan hai. File ko Notepad ya kisi code editor mein kholo aur ye dhundo:

| Kya badalna hai | Kya search karein |
| --- | --- |
| Naam | `Neetu` (kai jagah aata hai, find and replace karo) |
| Photo ka caption | `class="cap"` |
| Quote | `class="shy"` |
| Aakhri note | `class="note"` |
| Start screen ka text | `Ek chhota sa surprise` |

Badalne ke baad file ka naam `index.html` hi rehne do aur dobara upload kar do.

## Browser support

Naye Chrome, Safari, Edge aur Firefox par chalta hai, phone aur laptop dono par. Fonts Google Fonts se aate hain, toh bina internet ke bhi chalega, bas fonts default ho jayenge.

## Sab kuch ek jagah

| File | Kaam |
| --- | --- |
| `index.html` | Poora slideshow (design, photos, videos, song, code) |
| `og.jpg` | WhatsApp link preview ka birthday card |
| `README.md` | Ye guide |
