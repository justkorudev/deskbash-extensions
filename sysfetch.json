{
    "name": "SysFetch",
    "version": "1.0",
    "description": "Fetches system information",
    "url": "https://justkoru.github.io/deskbash-extensions/sysfetch.json",
    "commands": {
        "sysfetch": () => {
            const sysInfo = {
                'OS': "DeskBash v" + version,
                'Screen resolution': `${screen.width}x${screen.height}`,
                'Available screen width': screen.availWidth,
                'Available screen height': screen.availHeight,
                'Color depth': screen.colorDepth,
                'Pixel depth': screen.pixelDepth,
                'Online status': navigator.onLine,
                'Do not track': navigator.doNotTrack,
            };
            let sysInfoString = '';
            for (const [key, value] of Object.entries(sysInfo)) {
                sysInfoString += `${key}: ${value}<br>`;
            }
            console.log(sysInfoString);
            document.getElementById('cli-output').innerHTML += `<div>${sysInfoString}</div>`;
        }
    }
}
