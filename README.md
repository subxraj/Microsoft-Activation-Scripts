<p align="center"><img src="https://iili.io/K2774Og.png" alt="Subh Profile"></p>

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
