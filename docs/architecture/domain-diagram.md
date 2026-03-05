<div class="arch-diagram">

  <!-- Governance overlay -->
  <div class="arch-governance">
    <div class="arch-box arch-box--governance">
      <div class="arch-title">Governance &amp; Policy</div>
      <div class="arch-sub">IAM · Change Control · AI Oversight</div>
    </div>
  </div>

  <!-- Layers -->
  <div class="arch-layer">
    <div class="arch-layer__label">Entry</div>
    <div class="arch-row">
      <div class="arch-box">
        <div class="arch-title">External Partner / Client</div>
      </div>

      <div class="arch-arrow">→</div>

      <div class="arch-box">
        <div class="arch-title">External Interface</div>
        <div class="arch-sub">Auth · Validation · Idempotency</div>
      </div>
    </div>
  </div>

  <div class="arch-layer">
    <div class="arch-layer__label">Core Processing</div>
    <div class="arch-row">
      <div class="arch-box arch-box--wide">
        <div class="arch-title">Transaction Execution</div>
        <div class="arch-sub">Deterministic Workflow Engine</div>
      </div>
    </div>
  </div>

  <div class="arch-layer">
    <div class="arch-layer__label">Record &amp; Operations</div>
    <div class="arch-row arch-row--split">
      <div class="arch-box">
        <div class="arch-title">Ledger &amp; Financial Record</div>
        <div class="arch-sub">System of Record</div>
      </div>

      <div class="arch-box">
        <div class="arch-title">Risk &amp; Exception Operations</div>
        <div class="arch-sub">Human Workflow · Case Mgmt</div>
      </div>
    </div>

    <div class="arch-connectors">
      <div class="arch-conn">
        <span class="arch-conn__from">Transaction Execution</span>
        <span class="arch-conn__arrow">→</span>
        <span class="arch-conn__to">Ledger</span>
      </div>
      <div class="arch-conn">
        <span class="arch-conn__from">Transaction Execution</span>
        <span class="arch-conn__arrow">→</span>
        <span class="arch-conn__to">Operations</span>
      </div>
      <div class="arch-conn">
        <span class="arch-conn__from">Operations</span>
        <span class="arch-conn__arrow">→</span>
        <span class="arch-conn__to">Ledger</span>
      </div>
    </div>
  </div>

  <div class="arch-layer">
    <div class="arch-layer__label">Intelligence &amp; Evidence</div>
    <div class="arch-row arch-row--split">
      <div class="arch-box">
        <div class="arch-title">AI Advisory Plane</div>
        <div class="arch-sub">Summarize · Classify · Recommend</div>
      </div>

      <div class="arch-box">
        <div class="arch-title">Data &amp; Evidence Plane</div>
        <div class="arch-sub">Events · Metrics · Audit Logs</div>
      </div>
    </div>

    <div class="arch-connectors">
      <div class="arch-conn">
        <span class="arch-conn__from">Operations</span>
        <span class="arch-conn__arrow">↔</span>
        <span class="arch-conn__to">AI Advisory</span>
      </div>
      <div class="arch-conn">
        <span class="arch-conn__from">Core / Ledger / Ops / AI</span>
        <span class="arch-conn__arrow">→</span>
        <span class="arch-conn__to">Evidence Plane</span>
      </div>
    </div>
  </div>

</div>