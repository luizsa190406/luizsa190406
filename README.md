<svg fill="none" viewBox="0 0 600 240" width="100%" xmlns="http://www.w3.org/2000/svg">
  <foreignObject width="100%" height="100%">
    <div xmlns="http://www.w3.org/1999/xhtml">
      <style>
        .terminal {
          background-color: #0d1117;
          border: 1px solid #30363d;
          border-radius: 8px;
          padding: 18px;
          font-family: 'Fira Code', 'Cascadia Code', monospace;
          font-size: 14px;
          color: #c9d1d9;
          box-shadow: 0 10px 30px rgba(0,0,0,0.5);
        }
        .header { display: flex; gap: 8px; margin-bottom: 16px; }
        .dot { width: 12px; height: 12px; border-radius: 50%; }
        .red { background-color: #ff5f56; }
        .yellow { background-color: #ffbd2e; }
        .green { background-color: #27c93f; }
        
        .user { color: #a5d6ff; font-weight: bold; }
        .host { color: #79c0ff; }
        .dir { color: #d2a8ff; }
        .cmd { color: #f0883e; }
        .output { color: #c9d1d9; padding-left: 4px; }
        .folder { color: #79c0ff; font-weight: bold; }

        /* Animação de aparição linha por linha */
        .line { opacity: 0; animation: fadeIn 0.1s forwards; }
        .l1 { animation-delay: 0.2s; }
        .l2 { animation-delay: 0.8s; }
        .l3 { animation-delay: 1.4s; }
        .l4 { animation-delay: 2.0s; }
        .l5 { animation-delay: 2.4s; }

        .cursor {
          display: inline-block;
          width: 8px;
          height: 15px;
          background: #58a6ff;
          margin-left: 4px;
          vertical-align: middle;
          animation: blink 0.8s infinite;
        }

        @keyframes fadeIn { to { opacity: 1; } }
        @keyframes blink { 50% { opacity: 0; } }
      </style>

      <div class="terminal">
        <div class="header">
          <div class="dot red"></div>
          <div class="dot yellow"></div>
          <div class="dot green"></div>
        </div>
        
        <div class="line l1">
          <span class="user">luizsa190406</span><span class="host">@earth</span>:<span class="dir">~</span>$ <span class="cmd">whoami</span>
        </div>
        
        <div class="line l2 output">
          IT Intern @ Unicamp
        </div>
        
        <div class="line l3" style="margin-top: 8px;">
          <span class="user">luizsa190406</span><span class="host">@earth</span>:<span class="dir">~</span>$ <span class="cmd">ls ~/research</span>
        </div>
        
        <div class="line l4 output">
          <span class="folder">red-team/</span> &nbsp; <span class="folder">ai-sec/</span> &nbsp; <span class="folder">privacy/</span>
        </div>
        
        <div class="line l5" style="margin-top: 8px;">
          <span class="user">luizsa190406</span><span class="host">@earth</span>:<span class="dir">~</span>$ <span class="cursor"></span>
        </div>
      </div>
    </div>
  </foreignObject>
</svg>
