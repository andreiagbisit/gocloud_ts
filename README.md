<h1>⏰ GOCLOUD Timekeeping System</h1>

<p>
A Django-based <strong>timekeeping management system</strong> built for <strong>GOCLOUD Inc.</strong> as an internship project.<br>
It efficiently tracks employee and intern <strong>time-in</strong> and <strong>time-out</strong> activities while providing a secure and user-friendly interface for administrators.
</p>

<hr>

<h2>⚙️ I. Requirements</h2>

<h3>🐍 1. Python 3.12.8</h3>
<ul>
  <li>Download from <a href="https://www.python.org/downloads/release/python-3128/">Python.org</a>.</li>
  <li>Choose <strong>Windows Installer (64-bit)</strong>.</li>
  <li>✅ Tick “Add python.exe to PATH” during installation.</li>
</ul>

<h3>🗄️ 2. MySQL 8.0</h3>
<ul>
  <li>Download <strong>mysql-installer-community-8.0.x.x.msi</strong> from <a href="https://dev.mysql.com/downloads/installer/">MySQL Downloads</a>.</li>
  <li>Choose setup type <strong>Full</strong>.</li>
  <li>Use a custom port (e.g., <code>3307</code>) to avoid potential conflicts with web servers installed on your machine, if you have any (e.g.: XAMPP).</li>
  <li>You may also use a different X protocol port other than the provided default (e.g.: you may use <code>33061</code> instead of <code>33060</code>).</li>
</ul>

<hr>

<h2>💻 II. Local Setup</h2>

<h3>🧱 1. Create a Virtual Environment</h3>
<pre><code>python -m venv venv
</code></pre>

<h3>⚡ 2. Activate / Deactivate Virtual Environment</h3>
<pre><code>venv\Scripts\activate
deactivate
</code></pre>

<h3>📦 3. Install Dependencies</h3>
<pre><code>pip install -r requirements.txt
</code></pre>

<hr>

<h2>🧾 III. Environment Variables (.env Format)</h2>
<pre><code>DB_NAME=your_database_name
DB_USER=your_username
DB_PASSWORD=your_password
DB_HOST=localhost
DB_PORT=3307

EMAIL_PORT=587
EMAIL_USE_TLS=True
FP_EMAIL_HOST_USER=youremail@gmail.com
FP_EMAIL_HOST_PASSWORD=your_email_app_password
FP_DEFAULT_FROM_EMAIL=youremail@gmail.com

RECAPTCHA_PUBLIC_KEY=your_recaptcha_v2_site_key
RECAPTCHA_PRIVATE_KEY=your_recaptcha_v2_secret_key
</code></pre>

<p>🔹 To create Google reCAPTCHA v2 keys:  
<a href="https://cloud.google.com/recaptcha/docs/create-key-website">https://cloud.google.com/recaptcha/docs/create-key-website</a></p>

<blockquote>💡 Add <code>localhost</code> and <code>127.0.0.1</code> as valid domains for local testing.</blockquote>

<hr>

<h2>🚀 IV. Features</h2>
<ul>
  <li>✅ <strong>Employee and Intern Management</strong> with unique ID generation</li>
  <li>✅ <strong>Secure Login System</strong> with password reset via email (SMTP)</li>
  <li>✅ <strong>Google reCAPTCHA v2 Integration</strong> for bot protection</li>
  <li>✅ <strong>Responsive System UI</strong> for both employees and administrators</li>
  <li>✅ <strong>CRUD-Based Account and User Activity Management</strong></li>
  <li>✅ <strong>Downloadable Employee Time In/Out Activity Logs via PDF</strong> (powered by <strong>ReportLab</strong>)</li>
  <li>✅ <strong>Soft Deletion System</strong> for safe record management</li>
</ul>

<hr>

<h2>💻 📦 V. Technologies Used</h2>

<table border="1" cellpadding="6">
  <tr><th>Category</th><th>Technologies</th></tr>
  <tr><td><strong>Framework</strong></td><td>Django 5.1.5</td></tr>
  <tr><td><strong>Database</strong></td><td>MySQL 8.0 (<code>mysqlclient</code>)</td></tr>
  <tr><td><strong>Styling & UI</strong></td><td><a href="https://github.com/farridav/django-jazzmin">Jazzmin</a>, Bootstrap 4</td></tr>
  <tr><td><strong>Environment Management</strong></td><td><code>django-environ</code></td></tr>
  <tr><td><strong>Security</strong></td><td>Google reCAPTCHA v2 (<code>django-recaptcha</code>)</td></tr>
  <tr><td><strong>Data Handling</strong></td><td><code>pandas</code>, <code>numpy</code>, <code>openpyxl</code></td></tr>
  <tr><td><strong>PDF Generation</strong></td><td><code>reportlab</code></td></tr>
  <tr><td><strong>Image Processing</strong></td><td><code>pillow</code></td></tr>
  <tr><td><strong>HTTP Requests</strong></td><td><code>requests</code></td></tr>
</table>

<hr>

<h2>🧑‍💻 VI. Author & Credits</h2>
<p><strong>Developed by:</strong><br>
👨‍💻 AUF CCS GOCLOUD Internship Team (2025)<br>
</p>
