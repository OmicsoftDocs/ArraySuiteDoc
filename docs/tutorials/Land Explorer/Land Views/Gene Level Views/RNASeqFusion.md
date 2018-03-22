# RNA SEQ Fusion

## RNASeq Somatic Mutation Distribution View in Land Portal

![LandPortal_login_png](../../images/RNAseqFusion.png)

This view shows a series of charts of potential fusions for the specified gene or genes.

X-axis represents Fusion RPKM. RPKM is defined as seed reads per kilobase of seed region and per million mapped reads.
Y-axis is organized by grouping (e.g. Tumor Type).
Use the Sample tab to further filter the data using any associated sample/subject meta data.
Use the Fusion tab to filter the shown fusions. By default, all potential fusions are shown.

Suggested filters would be SplicePatternClass (remove non-canonical junctions), FrameShiftClass (remove frame shift and undefined fusions) and OnExonBoundary (look for fusions where both ends of fusion are on the exon boundary).

Potential real fusions are not likely to be in many normal samples. As a result, coloring has been automatically set to Sample Type.
Select Fusions in the plot and choose Fusion Details to see the full table for selected fusion.
