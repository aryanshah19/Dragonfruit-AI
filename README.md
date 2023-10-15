# Dragonfruit-AI

## Summary of Compression Techniques

The table below summarizes the sizes of the original and compressed images using Run-Length Encoding (RLE), Lempel-Ziv-Welch (LZW), and Bit Packing compression techniques, along with their respective Compression Ratios:

| Image Type | Original Size (bytes) | RLE Compressed Size (bytes) | RLE Compression Ratio | LZW Compressed Size (bytes) | LZW Compression Ratio | Bit Packing Compressed Size (bytes) | Bit Packing Compression Ratio |
|------------|-----------------------|-----------------------------|----------------------|-----------------------------|----------------------|-------------------------------------|-------------------------------|
| Blob       | 10128                 | 1176                        | 8.61                 | 2520                        | 4.02                 | 1250                                | 8.10                          |
| Dye        | 10128                 | 6072                        | 1.67                 | 4216                        | 2.40                 | 1250                                | 8.10                          |

These metrics enable a comprehensive evaluation of the efficiency of each compression technique in reducing image size while maintaining the quality and integrity of the image data.


### Observations:

- **RLE**: 
  - **Blob**: The size reduced significantly from 10128 bytes to 1176 bytes.
  - **Dye**: The size was reduced from 10128 bytes to 6072 bytes.
- **LZW**:
  - **Blob**: The size was reduced from 10128 bytes (original) to 2520 bytes.
  - **Dye**: The size was reduced from 10128 bytes to 4216 bytes.
- **Bit Packing**:
  - **Blob**: The size was reduced from 10128 bytes to 1250 bytes.
  - **Dye**: The size was reduced from 10128 bytes to 1250 bytes.

### Conclusion:

All three compression techniques - RLE, LZW, and Bit Packing - were able to compress the images to a smaller size. RLE provided substantial compression for the blob image, LZW was more effective for the dye image, and Bit Packing offered a consistent compression for both image types. 


### Tools and Techniques Employed:

#### 1. **Image Generation and Manipulation**
   - **Tool/Module:** OpenCV and NumPy
   - **Techniques:**
     - Utilizing NumPy for array manipulations and creating image masks.
     - Using OpenCV for drawing shapes, managing image data, and for visual analysis through plots.

#### 2. **Data Representation and Visualization**
   - **Tool/Module:** Matplotlib
   - **Techniques:**
     - Used to visualize generated images and to provide comparative visuals of the generated blobs and dye distribution.
     - Employed for overlaying color masks to highlight regions of interest (e.g., dye within the parasite blob).

#### 3. **Logical Structuring and Data Management**
   - **Technique:** Conditional Logic and Loop Structures
   - **Approach:**
     - Used loops to create repetitions in image generation, ensuring variations.
     - Employed conditional logic to evaluate scenarios where dye proportion exceeds a certain threshold, indicating a condition akin to cancer.

#### 4. **Time Complexity Optimization**
   - **Tool/Module:** Time
   - **Techniques:**
     - Used to measure and compare execution times between different implementation versions.
     - Supported in making informed decisions regarding computational efficiency.

#### 5. **Algorithm Optimization**
   - **Technique:** Minimal Data Storage and Efficient Computations
   - **Approach:**
     - Devised methods to store only essential data (e.g., parasite pixels) to optimize memory usage.
     - Employed vectorized operations via NumPy to minimize the computational cost of pixel-level operations.



### Leveraging Large Language Models (LLM):

#### A. **Logical Approach:**
   - **Problem Decomposition:** Breaking down the overarching challenge into sub-tasks and addressing them modularly (e.g., image creation, visualization, cancer detection).
   - **Conditional Logic:** Establishing thresholds and using logical conditions to derive conclusions (e.g., whether the parasite has a cancer-like condition based on dye percentage).
   - **Loop Structures:** Utilizing loops for repetitive tasks and iterations, ensuring diversification in generated images.
   
#### B. **Learning Approach:**
   - Although direct machine learning techniques were not explicitly utilized in the provided solutions, foundational approaches align with learning methodologies.
   - **Data Generation:** The creation of synthetic image data can be likened to data augmentation in learning models.

   
### Conclusion:

Through a blend of image processing techniques, logical structuring, visualization tools, and considering optimization for storage and computation, the challenge was addressed in a systematic and structured manner. While the primary methodologies were focused on logical approaches and structured programming, the underlying concepts and structuring lend themselves cohesively to a learning-based approach and could be further extended towards a model-oriented solution with additional complexities and data.
