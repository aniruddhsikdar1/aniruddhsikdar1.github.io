<div class="dataset-item" style="display: flex; flex-direction: row-reverse; align-items: flex-start; gap: 1.5em;">
  
  <!-- Image on the right (same image & size) -->
  <div class="dataset-media">
    <img src="/assets/images/gta_2.drawio.png" alt="Robotic Manipulation">
  </div>

  <!-- Existing content (unchanged) -->
  <div style="display: flex; flex-direction: column; gap: 1em;">

    <div class="dataset-content">
      
      <!-- Legend / Title -->
      <div style="display: flex; align-items: center; flex-wrap: wrap; gap: 0.5em;">
        <span style="
          background-color: #007BFF;
          color: white;
          padding: 5px 12px;
          border-radius: 16px;
          font-size: 0.85em;
          font-family: 'Segoe UI', Arial, sans-serif;
          box-shadow: 0 2px 5px rgba(0,0,0,0.15);
          white-space: nowrap;
        ">
          Course Project
        </span>
        <strong>One-Shot Object Localization for Robotic Manipulation</strong>
      </div>

      <ul>
        <li>Addressed the challenge of localizing novel objects from a single visual cue without prior object-specific training.</li>
        <li>Enabled robotic pick-and-place in unstructured environments through vision-based one-shot localization.</li>
        <li>Implemented a Siamese CNN with shared weights to learn similarity between cue and scene images.</li>
        <li>Designed a spatial attention mechanism to extract object-specific features from the cue image.</li>
        <li>Generated similarity score maps and applied SoftArgMax to accurately predict object coordinates.</li>
        <li>Integrated vision-based localization with inverse kinematics control for robotic picking in both simulation and real hardware.</li>
      </ul>

    </div>
  </div>
</div>
