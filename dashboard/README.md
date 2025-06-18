WHAT IS DASHBOARD?

Dashboard is a program designed to run on a mobile browser.
When run, it presents the user with a series of buttons.
Pressing a button generates an on-screen output that relates to
the title of the button.

HOW DO I ADD MORE / AMEND THE BUTTONS?

Open the code in a code editor (Microsoft Visual Studio Code is recommended)
Scroll down to the main code.

Each button functionality roughly follows the same format;

In the "button-row" div (at the start of the body section) add a button.

EG/     <button class="hack-button" onclick="startHack('log')">Deploy Reverse Shell</button>

Instead of "startHack('log')" - Replace log with a single word descriptor for your function
Instead of >Deploy Reverse Shell</button> - Give your buton a new 'title'

In the const sequences = { array (at the start of the Script element) add your data

EG      title: "Reverse Shell Deployment",
        log: [
          "[*] Target located at 192.168.1.42",
          "[*] Generating tcp/reverse_shell binary...",
          "[+] Binary ready. Size: 23.4KB",
          "[*] Deploying to target system...",
          "[+] Binary executed successfully.",
          "[*] Awaiting reverse shell...",
          "[+] Remote session established."
        ],
        final: "ACCESS GRANTED"
      },

Instead of title: "Reverese Shell Deployment", - Replace this with a title for the function
Instead of log: [ - Replace this with the single word descriptor from earlier
Amend the contents of the 'log' array to the comments desired.
Instead of final: "ACCESS GRANTED" - Replace this with the final outcome message desired.

Once the function runs it it will pause for a moment before returning you to the menu.

ANYTHING ELSE?

I don't think so?
