# YouTube Video Playback Proxy
This project provides a simple proxy server to facilitate YouTube video playback in applications that may have restrictions or limitations on direct access to YouTube content. By routing requests through this proxy, your users can enjoy uninterrupted video streaming.

I wrote this because I needed to enable YouTube embed playback on iOS, and apparently Apple or Google broke the embedding process. Adding the Referrer and Origin headers did not fix the issue, but routing the requests through this proxy worked.

Based on discussions in the following Stackoverflow post:

https://stackoverflow.com/questions/79802987/youtube-error-153-video-player-configuration-error-when-embedding-youtube-video

And to address the following Google API issue:

https://issuetracker.google.com/issues/457483150

# Features
- Simple setup and configuration - just edit the Index.cshtml and _Layout.cshtml to your liking.
- Output caching.
- Simple and lightweight design.

# Requirements
- .NET 10
- ASP.NET Core

Why .NET? Because I knew what I wanted to write and I knew how to write it quickly in .NET. Feel free to port it to your favorite language/framework.

# License
Apache License 2.0. See license file for details. You use this software at your own risk. No warranties, etc.

# Usage
Pass the YouTube video ID as a query parameter to the proxy server. For example:
```
http://your-proxy-server.com/?v=YOUR_VIDEO_ID
```

Replace `YOUR_VIDEO_ID` with the actual ID of the YouTube video you want to play.

That's it! Your application should now be able to play YouTube videos through the proxy server without any issues. If it no longer works, please check for updates to this project or consider alternative solutions. 

# Contact
If you have any questions or need further assistance, feel free to reach out or open an issue on the project's GitHub repository.

My LinkedIn: https://www.linkedin.com/in/aurirahimzadeh/

# Contributing
Contributions are welcome! If you find a bug or have a feature request, please open an issue or submit a pull request on GitHub.

# Acknowledgments
Thanks to the developers and community members who discussed this issue on Stackoverflow and the Google Issue Tracker, helping to shed light on the problem and potential solutions.

# Disclaimer
This project is provided "as is" without any warranties or guarantees. Use it at your own risk. The author is not responsible for any issues that may arise from using this proxy server.

**This was a quick fix for a specific problem and may not be a permanent solution.**
