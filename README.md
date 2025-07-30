# Copy from URL

A minimal HTML + JavaScript page that automatically copies a value from the URL query parameter to the clipboard when the page loads, then attempts to close the tab or redirect to about:blank.

## Usage

Simply append a `data` parameter to the URL:

```
https://your-domain.vercel.app/?data=XYZ123
```

The page will:
1. Extract the value from the `data` query parameter
2. Copy it to the clipboard
3. Show a success/error status
4. Attempt to close the tab
5. If closing fails, redirect to `about:blank`

## Features

- ✅ Mobile-friendly responsive design
- ✅ Modern clipboard API with fallback for older browsers
- ✅ Visual feedback with loading/success/error states
- ✅ Graceful error handling
- ✅ Production-ready for Vercel deployment
- ✅ Minimal and lightweight

## Deployment

This project is ready to deploy on Vercel:

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Deploy automatically

The `vercel.json` configuration ensures proper routing and static file serving.

## Browser Compatibility

- Modern browsers with clipboard API support
- Fallback for older browsers using `document.execCommand`
- Works on both desktop and mobile devices

## Security Notes

- Requires HTTPS for clipboard API to work
- Uses secure context detection
- Minimal attack surface with no external dependencies 