### BOGausS: Better Optimized Gaussian Splatting
BOGausS proposes an improved training strategy with the following contributions:
<ul>
  <li><strong>Confidence-aware updates:</strong> Bayesian confidence sets a minimum Gaussian size and scales gradients by distance, preventing oversampling and accelerating convergence.</li>
  <li><strong>Unbiased Sparse Adam:</strong> Reformulated optimizer yields unbiased moment estimates and inherits state after splits for smoother training.</li>
  <li><strong>Density-preserving splits:</strong> Splits along the longest axis, adjusting size and opacity to keep total density constant and the loss curve smooth.</li>
  <li><strong>Rate-distortion densification:</strong> Prioritises splits by reconstruction error and prunes by effective opacity for compact, high-quality models.</li>
  <li><strong>Optional exposure correction</strong> refines appearance under photometric inconsistencies.</li>
</ul>