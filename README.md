# apex
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Project Scope Questionnaire - APEX</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@tabler/icons@latest/tabler-icons.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    
    body {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
      background: #f5f5f5;
      padding: 2rem 1rem;
      line-height: 1.6;
    }
    
    .container {
      max-width: 600px;
      margin: 0 auto;
      background: white;
      border-radius: 12px;
      padding: 2rem;
      box-shadow: 0 1px 3px rgba(0,0,0,0.1);
    }
    
    h1 {
      font-size: 22px;
      font-weight: 500;
      margin-bottom: 0.5rem;
      color: #222;
    }
    
    .subtitle {
      font-size: 14px;
      color: #666;
      margin-bottom: 2rem;
    }
    
    .form-section {
      margin-bottom: 2rem;
    }
    
    .form-section label {
      font-size: 14px;
      font-weight: 500;
      color: #222;
      display: block;
      margin-bottom: 0.75rem;
    }
    
    .radio-group, .checkbox-group {
      display: flex;
      flex-direction: column;
      gap: 8px;
    }
    
    .checkbox-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 8px;
    }
    
    input[type="radio"],
    input[type="checkbox"] {
      cursor: pointer;
      accent-color: #378ADD;
    }
    
    .radio-group label,
    .checkbox-group label,
    .checkbox-grid label {
      display: flex;
      align-items: center;
      gap: 8px;
      cursor: pointer;
      font-size: 14px;
      font-weight: 400;
      color: #333;
    }
    
    textarea {
      width: 100%;
      min-height: 80px;
      padding: 12px;
      border: 1px solid #ddd;
      border-radius: 8px;
      font-size: 14px;
      font-family: inherit;
      resize: vertical;
      font-weight: 400;
    }
    
    textarea:focus {
      outline: none;
      border-color: #378ADD;
      box-shadow: 0 0 0 2px rgba(55, 138, 221, 0.1);
    }
    
    .button-group {
      display: flex;
      gap: 8px;
      margin-top: 2rem;
    }
    
    button {
      flex: 1;
      padding: 12px 16px;
      border: 1px solid #ddd;
      background: white;
      border-radius: 8px;
      cursor: pointer;
      font-size: 14px;
      font-weight: 500;
      color: #222;
      transition: all 0.2s;
    }
    
    button:hover {
      background: #f9f9f9;
      border-color: #999;
    }
    
    button:active {
      transform: scale(0.98);
    }
    
    .summary-box {
      background: #f9f9f9;
      border: 1px solid #ddd;
      border-radius: 8px;
      padding: 12px;
      font-size: 13px;
      color: #666;
      line-height: 1.6;
      margin-top: 1rem;
      display: none;
      cursor: pointer;
      transition: all 0.2s;
    }
    
    .summary-box:hover {
      background: #f0f0f0;
      border-color: #999;
    }
    
    .summary-box strong {
      color: #222;
      display: block;
      margin-bottom: 8px;
    }
    
    .hidden {
      display: none;
    }
    
    .success-message {
      background: #e8f5e9;
      border: 1px solid #81c784;
      border-radius: 8px;
      padding: 12px;
      color: #2e7d32;
      font-size: 14px;
      text-align: center;
      margin-top: 1rem;
      display: none;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Project scope questionnaire</h1>
    <p class="subtitle">Quick 2-minute form to finalize your project focus</p>
    
    <form id="scopeForm">
      <!-- Product line -->
      <div class="form-section">
        <label>Which product line?</label>
        <div class="radio-group">
          <label>
            <input type="radio" name="product" value="Clothing" required>
            <span>Clothing</span>
          </label>
          <label>
            <input type="radio" name="product" value="Accessories">
            <span>Accessories (bucket hat, scarf, etc)</span>
          </label>
          <label>
            <input type="radio" name="product" value="Skincare & candles">
            <span>Skincare & candles</span>
          </label>
        </div>
      </div>

      <!-- Gender group (conditional) -->
      <div class="form-section hidden" id="gender-section">
        <label>Target gender group?</label>
        <div class="radio-group">
          <label>
            <input type="radio" name="gender" value="Male">
            <span>Male</span>
          </label>
          <label>
            <input type="radio" name="gender" value="Female">
            <span>Female</span>
          </label>
          <label>
            <input type="radio" name="gender" value="Both / Unisex">
            <span>Both / Unisex</span>
          </label>
        </div>
      </div>

      <!-- Markets -->
      <div class="form-section">
        <label>Target markets (pick 1-2)</label>
        <div class="checkbox-grid">
          <label>
            <input type="checkbox" name="markets" value="US">
            <span>US</span>
          </label>
          <label>
            <input type="checkbox" name="markets" value="Canada">
            <span>Canada</span>
          </label>
          <label>
            <input type="checkbox" name="markets" value="Australia">
            <span>Australia</span>
          </label>
          <label>
            <input type="checkbox" name="markets" value="New Zealand">
            <span>New Zealand</span>
          </label>
          <label>
            <input type="checkbox" name="markets" value="UK">
            <span>UK</span>
          </label>
          <label>
            <input type="checkbox" name="markets" value="Japan">
            <span>Japan</span>
          </label>
          <label>
            <input type="checkbox" name="markets" value="Hong Kong">
            <span>Hong Kong</span>
          </label>
          <label>
            <input type="checkbox" name="markets" value="Singapore">
            <span>Singapore</span>
          </label>
        </div>
      </div>

      <!-- Additional competitor categories -->
      <div class="form-section">
        <label>Any additional competitor categories?</label>
        <textarea id="competitors" placeholder="E.g. 'Asian heritage brands' or 'sustainable luxury'..."></textarea>
      </div>

      <!-- Buttons -->
      <div class="button-group">
        <button type="button" id="copy-btn" onclick="copySummary()">
          <i class="ti ti-copy" style="margin-right: 6px;"></i>Copy summary
        </button>
        <button type="button" id="email-btn" onclick="openEmail()">
          <i class="ti ti-mail" style="margin-right: 6px;"></i>Email response
        </button>
      </div>

      <!-- Summary preview -->
      <div class="summary-box" id="summary">
        <strong>Your response:</strong>
        <span id="summary-text"></span>
      </div>

      <!-- Success message -->
      <div class="success-message" id="successMsg">✓ Copied to clipboard!</div>
    </form>
  </div>

  <script>
    const productRadios = document.querySelectorAll('input[name="product"]');
    const genderSection = document.getElementById('gender-section');
    const genderRadios = document.querySelectorAll('input[name="gender"]');
    const marketCheckboxes = document.querySelectorAll('input[name="markets"]');
    const competitorsTA = document.getElementById('competitors');
    const summaryDiv = document.getElementById('summary');
    const summaryText = document.getElementById('summary-text');
    const copyBtn = document.getElementById('copy-btn');
    const emailBtn = document.getElementById('email-btn');
    const successMsg = document.getElementById('successMsg');

    // Show gender section when product selected
    productRadios.forEach(radio => {
      radio.addEventListener('change', () => {
        genderSection.classList.remove('hidden');
        updateSummary();
      });
    });

    // Update on gender change
    genderRadios.forEach(radio => {
      radio.addEventListener('change', updateSummary);
    });

    // Limit markets to 2
    marketCheckboxes.forEach(checkbox => {
      checkbox.addEventListener('change', () => {
        const checked = document.querySelectorAll('input[name="markets"]:checked').length;
        if (checked > 2) {
          alert('Please select maximum 2 markets');
          checkbox.checked = false;
        }
        updateSummary();
      });
    });

    competitorsTA.addEventListener('input', updateSummary);

    function updateSummary() {
      const product = document.querySelector('input[name="product"]:checked')?.value || '—';
      const gender = document.querySelector('input[name="gender"]:checked')?.value || '—';
      const markets = Array.from(document.querySelectorAll('input[name="markets"]:checked'))
        .map(c => c.value)
        .join(', ') || '—';
      const competitors = competitorsTA.value || 'None specified';
      
      const text = `Product line: ${product} | Target gender: ${gender} | Markets: ${markets} | Additional competitors: ${competitors}`;
      summaryText.textContent = text;
      summaryDiv.style.display = 'block';
    }

    function copySummary() {
      const text = summaryText.textContent;
      navigator.clipboard.writeText(text).then(() => {
        successMsg.style.display = 'block';
        setTimeout(() => successMsg.style.display = 'none', 2000);
      });
    }

    function openEmail() {
      const text = summaryText.textContent;
      const subject = 'Re: Project Scope Questionnaire - APEX';
      const body = encodeURIComponent(`Hi APEX team,\n\nHere are my responses:\n\n${text}\n\nBest regards`);
      window.location.href = `mailto:your-email@example.com?subject=${encodeURIComponent(subject)}&body=${body}`;
    }
  </script>
</body>
</html>
