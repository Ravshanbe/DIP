#  Practical Code Challenges – Image Filtering Lab

##  Challenge 1: Kernel Size Experiment
1. Apply the uniform (box) filter using different kernel sizes:
   - 3×3
   - 5×5
   - 9×9
2. Display the results side by side.
3. Describe how increasing kernel size affects:
   - Blur strength
   - Image details
   - Sharp edges

---

##  Challenge 2: Gaussian Sigma Investigation
1. Apply Gaussian blur with:
   - Small sigma (e.g., 1)
   - Medium sigma (e.g., 5)
   - Large sigma (e.g., 15)
2. Keep kernel size constant.
3. Observe and explain:
   - What role does sigma play?
   - How is Gaussian blur different from uniform blur visually?

---

##  Challenge 3: Manual Convolution
1. Create your own custom 3×3 kernel using NumPy.
2. Apply it using `cv2.filter2D()`.
3. Try:
   - A sharpening kernel
   - An edge detection kernel
4. Compare results with built-in filters.

---

##  Challenge 4: Noise Removal Test
1. Add artificial noise to the original image:
   - Gaussian noise
   - Salt-and-pepper noise
2. Apply:
   - Uniform filter
   - Gaussian filter
3. Which filter performs better for each noise type?
4. Justify your answer with visual comparison.

---

##  Challenge 5: Edge Preservation Study
1. Blur the image using:
   - Box filter
   - Gaussian filter
2. Compare how edges are affected.
3. Measure pixel intensity differences across edges before and after filtering.
4. Which method preserves structure better?

---

##  Challenge 6: Performance Comparison
1. Measure execution time for:
   - `cv2.filter2D()`
   - `cv2.GaussianBlur()`
2. Run each filter multiple times.
3. Calculate average processing time.
4. Which method is faster? Why?

---

##  Challenge 7: Kernel Normalization Test
1. Create a kernel that is NOT normalized (sum ≠ 1).
2. Apply it to the image.
3. Observe what happens to brightness.
4. Fix the issue by normalizing the kernel.

---

#  Final Challenge: Smart Filter Selector
Create a mini program that:
- Asks the user to choose:
  - Uniform filter
  - Gaussian filter
- Asks for kernel size and sigma (if Gaussian)
- Applies the selected filter
- Displays original and filtered images side by side
Make it structured, reusable, and well-commented.