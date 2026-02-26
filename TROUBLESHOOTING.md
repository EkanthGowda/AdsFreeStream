# 🔧 Troubleshooting Guide

## ⚠️ Error 153: Video Player Configuration Error

This error means **YouTube has blocked embedding** for your video. Here's how to fix it:

### Quick Fix (5 steps):

1. **Go to YouTube Studio**: https://studio.youtube.com
2. **Click "Content"** in the left sidebar
3. **Find your live stream** and click the **pencil icon** (Edit)
4. **Click "Show more"** at the bottom
5. **Find "Allow embedding"** → Make sure it's **✅ CHECKED**
6. **Click Save**
7. **Refresh your website**

### Why This Happens:

- ❌ YouTube defaults to **embedding disabled** for some accounts
- ❌ Stream must be **started** before you can enable embedding
- ❌ Video must be **Public** or **Unlisted** (not Private)

### Step-by-Step With Screenshots:

#### Step 1: Open YouTube Studio
Go to: https://studio.youtube.com

#### Step 2: Navigate to Content
Click "Content" in left menu → You'll see your videos/streams

#### Step 3: Edit Your Stream
Find your live stream → Click the **pencil/edit icon**

#### Step 4: Expand Advanced Settings
- Scroll down
- Click "Show more" or "Advanced settings"

#### Step 5: Enable Embedding
- Find the section called **"Allow embedding"**
- Make sure the checkbox is **CHECKED ✅**
- Click **SAVE**

#### Step 6: Test
- Refresh your website (Cmd/Ctrl + Shift + R)
- The stream should now appear!

---

## 🚨 Other Common Issues

### "This video is unavailable"

**Cause**: Stream hasn't started yet or video is private

**Fix**:
1. Start streaming in OBS first
2. Wait 10-20 seconds for YouTube to process
3. Refresh your website

### "Playback error" or black screen

**Cause**: Internet connection or YouTube processing delay

**Fix**:
1. Check your internet connection
2. Wait 30 seconds for YouTube to buffer
3. Hard refresh (Cmd/Ctrl + Shift + R)

### Stream not showing even after enabling embedding

**Fix**:
1. Check if stream is actually live on YouTube
2. Verify the VIDEO_ID is correct in your HTML
3. Try watching directly on YouTube first
4. Clear browser cache

### Low quality or buffering

**Fix in OBS**:
1. Settings → Output
2. Lower bitrate:
   - 720p: 3000-4500 kbps
   - 480p: 1500-2500 kbps
3. Reduce resolution in Video settings

---

## ✅ Verification Checklist

Before troubleshooting, verify:

- [ ] OBS is streaming
- [ ] YouTube Studio shows "Live" status
- [ ] Video visibility is Public or Unlisted (not Private)
- [ ] "Allow embedding" is enabled
- [ ] Correct VIDEO_ID in HTML file
- [ ] Browser is refreshed (hard refresh)

---

## 🆘 Still Not Working?

### Option 1: Direct Link (Temporary Solution)
Your website now includes a direct link to watch on YouTube:
- Click "Watch directly on YouTube" on your website
- This bypasses embedding entirely

### Option 2: Use Different Platform
If YouTube restrictions continue:
- Consider Twitch (allows embedding by default)
- Try Facebook Live
- Use Vimeo Live

### Option 3: Alternative Embed Method
Some creators use:
- YouTube Live chat embed (always works)
- Custom player solutions (more complex)

---

## 📞 Need More Help?

1. Check your [CHECKLIST.md](CHECKLIST.md)
2. Review [README.md](README.md) setup guide
3. Verify OBS settings

**Quick test**: Can you watch your stream directly on YouTube? If yes, it's an embedding issue. If no, it's a streaming issue.
