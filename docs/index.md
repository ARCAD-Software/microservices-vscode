<div class="hero">
  <img class="hero-logo" src="_media/microservices.ico" alt="ARCAD Transformer Microservices" />
  <h1>ARCAD Transformer Microservices</h1>
  <p class="tagline">RPG refactoring and REST web service creation for IBM i, right inside VSCode.</p>
  <div class="badges">
    <img src="https://img.shields.io/visual-studio-marketplace/v/arcadsoftware.arcad-microservices" alt="Marketplace version" />
    <img src="https://img.shields.io/visual-studio-marketplace/i/arcadsoftware.arcad-microservices" alt="Marketplace installs" />
  </div>
  <div class="hero-actions">
    <a class="btn btn-primary" href="#/installation">Get Started</a>
    <a class="btn btn-secondary" href="https://marketplace.visualstudio.com/items?itemName=arcadsoftware.arcad-microservices" target="_blank">Install from Marketplace</a>
  </div>
</div>

> [!TIP]
> **Version 1.0.3** is out now, compatible with **V26 Server** and later. See the [Version History](version-history.md) for the full list of changes.

## What is ARCAD Transformer Microservices?

ARCAD Transformer Microservices helps you modernize legacy IBM i applications by isolating reusable, unique sections of code and gradually evolving a monolithic codebase into a modular, microservices-friendly architecture.

It focuses on three things:

- **Auditing risk** before externalizing a selected piece of code
- **Locating usage** of that code across the application
- **Ensuring uniqueness**, so centralized code isn't duplicated once extracted

On top of that, it automates the deployment of REST web services for IBM i ILE objects via IBM's Integrated Web Services Server (IWS), and supports iUnit testing to validate quality after externalization.

<div class="card-grid">

<a class="card" href="#/rule">
  <span class="card-icon">📐</span>
  <h4>Rules</h4>
  <p>Define the analysis rules that drive extraction and similarity detection.</p>
</a>

<a class="card" href="#/project">
  <span class="card-icon">🗂️</span>
  <h4>Projects</h4>
  <p>Organize your rules and results into projects tied to your IBM i application.</p>
</a>

<a class="card" href="#/extractions">
  <span class="card-icon">✂️</span>
  <h4>Code Extraction</h4>
  <p>Analyze, extract, and externalize reusable pieces of RPG code.</p>
</a>

<a class="card" href="#/codesimilarity">
  <span class="card-icon">🧬</span>
  <h4>Code Similarity</h4>
  <p>Find duplicated or near-duplicate code across your application.</p>
</a>

<a class="card" href="#/webservices">
  <span class="card-icon">🌐</span>
  <h4>Web Services</h4>
  <p>Deploy ILE programs and service programs as REST web services with IWS.</p>
</a>

<a class="card" href="#/macro-commands">
  <span class="card-icon">⚙️</span>
  <h4>Macro Commands</h4>
  <p>Browse, run, and track macro commands and their execution history.</p>
</a>

</div>

## Why go microservices?

**For developers:**
- Avoids a large, unwieldy code base — easier to maintain and extend
- Faster deployments and shorter IDE load times
- Simpler debugging and dependency tracking

**For the business:**
- More frequent releases and shorter feedback cycles
- Better resource management and service availability
- Less duplicated code, lower maintenance cost

---

Need the server-side setup? See the <a href="ARCAD-TMS_26.0_A4_Installation~Guide.pdf" target="_blank">Microservices Server Installation Guide</a>, or reach out via [Contact Us](https://www.arcadsoftware.com/about/contact/).
