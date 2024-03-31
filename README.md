# aerosol

No-nonsense Twitch chat overlay that I use as an OBS browser source.

# Getting Started in [OBS Studio](https://obsproject.com/)

1. Create a browser source, and position/size it however you'd like. Personally, I like 400x600 px, and that's where I've tested it.
2. Set the URL to `https://addiment.github.io/aerosol/chat/?channel=<CHANNEL>`, and change &gt;CHANNEL&lt; to the name of the channel you want to display.

# Customization

If you're good with CSS, you should be fine. I reccommend reviewing the CSS in the index. Chat lines are stored in `div#chat-box`. Chat line markup looks like this:

```html
<div class="chat-line" data-nick="addiment_lc" data-time="4294967295" data-id="00000000-0000-0000-0000-000000000000">
 <div class="badge-box">
  <img class="badge">
 </div>
	 <span class="nick" style="color: #ff1040;">addiment_lc</span><span class="separator"></span><span class="message">test message! <img class="emote"></span>
</div>
```

# Features / Issues

- I don't plan on supporting raids, and I don't know whether or not they work.
- Deleted messages are removed from the chatbox, and clearing the chat should also work.
- Badges are planned, but require extra API setup that I don't particularly feel like doing right now.
- BetterTTV / FrankerFacez support is *planned,* but also requires extra setup that I also don't feel like doing.
- No reconnection right now, coming as soon as I get bothered by it.
