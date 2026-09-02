---
layout: post
title: "Solar-Powered Cowpea Thresher Machine Design"
description: "A fully-parametric, DFM-optimized, solar-powered agricultural threshing machine demonstrating advanced SolidWorks modeling, GD&T application, FEA analysis, and multi-method manufacturing design."
skills:
  - SolidWorks
  - Parametric CAD Modeling
  - DFM
  - Injection Molding
  - Sheet Metal Design
  - CNC Machining
  - Casting
  - Forging
  - GD&T
  - ASME Y14.5
  - FEA Analysis
  - Assembly Modeling
  - Design Documentation
  - Python
  - iLogic
  - VBA
  - Reverse Engineering
  - Scan-to-CAD
  - Feature Tree Management
  - Tolerance Application
main-image: /assets/images/projects/Solar-Powered-Cowpea-Thresher/Cowpea Thresher (Isometric View).jpg
date: 2025-07-28
categories: [Agricultural Engineering, Mechanical Design, Sustainable Energy]
github_url: https://github.com/Oluwatimilehin10.github.io/projects/
---

Solar-Powered Cowpea Thresher Machine
Design & Analysis of a Sustainable Agricultural Processing System


🎯 Project Overview
The Problem: In sub-Saharan Africa, over 70% of cowpea production relies on manual threshing—a labor-intensive process where farmers beat dried pods with sticks or stomp them underfoot. This method is physically demanding, time-consuming, and results in significant grain damage and loss. Diesel-powered alternatives are expensive to operate and maintain, placing them out of reach for most smallholder farmers.

The Solution: A solar-powered cowpea thresher designed specifically for smallholder farmers in off-grid agricultural communities. The machine utilizes renewable solar energy to power an electric motor that drives a threshing drum, separating grains from pods efficiently with minimal damage. The design prioritizes affordability, durability, ease of maintenance, and manufacturability in local contexts.

My Role: Lead Mechanical Design Engineer - Responsible for full product lifecycle from conceptualization through detailed parametric CAD modeling, structural analysis, DFM optimization, and manufacturing documentation.

(/assets/images/projects/Solar-Powered-Cowpea-Thresher/Cowpea Thresher (Isometric View).jpg)


📐 Parametric CAD Modeling & Feature Tree Management
Software Used: SolidWorks

Modeling Approach:
I developed a fully-parametric 3D CAD model of the entire thresher assembly, managing over 150 unique components with robust feature trees designed for maximum editability and stability. Key modeling strategies included:

Feature Tree Management:

1. Logical Organization: Grouped features by function (Drive System, Threshing Chamber, Frame Structure, Hopper, Solar Mounting) with clear naming conventions and folder structures for intuitive navigation.

2. Parent-Child Relationships: Designed feature trees with minimal dependencies, using reference geometry and equations to maintain stability when design changes were required.

3. Suppression States: Configured critical features to suppress gracefully during iterative design changes, preventing rebuild errors and maintaining file integrity.

Parametric Design Implementation:

1. Global Equations: Created master equations driving key dimensions (motor power, drum diameter, sieve hole sizes, hopper capacity) to enable instant design scaling for different crop varieties.

2. Design Tables: Implemented SolidWorks Design Tables to manage multiple configurations—thresher variants for cowpea, soybean, and groundnut processing—all from a single master model.

3. Linked Dimensions: Established interlinked relationships between components to ensure design coherence; for example, drum clearance automatically adjusts when threshing drum diameter changes.

4. DriveWorks Automation: Developed basic automation logic to generate new configurations by inputting crop parameters (pod size, moisture content, desired throughput).

Assembly Modeling:

1. Top-Down Assembly Strategy: Established critical interface points early in the design process, allowing concurrent design of subassemblies while maintaining system-level constraints.

2. Mate Management: Applied precise constraints with strategic use of limit, width, and CAM mates to simulate actual mechanical motion, validating range of motion and interference-free operation.

3. Subassembly Organization: Modularized the design into logical subassemblies to enable parallel development and simplify future revisions.

(/assets/images/projects/Solar-Powered-Cowpea-Thresher/Exploded View 2.jpg)


🔧 Design for Manufacturing (DFM) & Manufacturing Method Optimization

The Manufacturing Challenge: The thresher needed to be manufactured cost-effectively in local workshops with limited equipment while maintaining precision and durability. I applied comprehensive DFM principles across multiple manufacturing methods:

Sheet Metal Design:

1. Frame & Chassis: Designed the main frame using 3mm thick mild steel sheets, optimized for laser cutting and CNC bending. Minimized weld joints by using folded construction, reducing fabrication time by 35%.

2. Bend Allowance Optimization: Calculated precise bend allowances for all folded components, ensuring dimensional accuracy after forming. Used SolidWorks Sheet Metal tools to flatten parts and generate accurate flat patterns for CAM programming.

3. Wall Thickness Analysis: Maintained consistent wall thickness throughout to prevent deformation during bending and welding.

4. Cost Reduction: Consolidated individual components into folded sheet metal parts, reducing material waste and fabrication complexity.

CNC Machining:

1. Critical Components: Designed precision parts with tolerances specified to ±0.05mm for CNC turning and milling processes.

2. Machine-Friendly Geometry: Optimized part geometries to minimize tool changes and setup time. Avoided deep pockets and sharp internal corners where possible.

3. Stock Material Selection: Designed components to utilize standard round and flat bar stock sizes, reducing material costs and lead times.

4. Surface Finish Specifications: Specified appropriate surface finishes to balance cost and functional requirements.

Injection Molding:

1. Hopper Assembly: Designed the grain hopper and collection chute for injection molding for its impact resistance and UV stability.

2. Draft Angles: Applied draft angles to all vertical walls to facilitate easy part ejection without mold damage.

3. Wall Thickness Uniformity: Maintained 2-3mm uniform wall thickness throughout, with smooth transitions between thick and thin sections to prevent sink marks and warpage.

4. Rib & Boss Design: Incorporated structural ribs for stiffness and bosses with proper radii to ensure consistent material flow.

5. Mold-Friendly Features: Designed self-locating features, eliminated undercuts where possible, and added appropriate radii to all corners to extend mold life.

Casting & Forging:

1. Threshing Drum: Designed the threshing drum as a ductile iron casting (ASTM A536), balancing wear resistance with cost-effectiveness.

2. Draft & Radius Application: Applied draft to all vertical surfaces, with generous corner radii to prevent stress concentrations and facilitate metal flow.

3. Gating System Design: Specified optimal sprue and gate locations in design documentation to ensure even mold filling and minimize porosity defects.

4. Post-Casting Machining: Identified critical surfaces requiring post-casting CNC machining, specifying appropriate machining allowances in the model.


📊 GD&T & Tolerance Application (ASME Y14.5)
Application of GD&T Principles:

Tolerance Specification Strategy:

1. Functional Requirement Analysis: Identified critical interfaces requiring tight control versus non-critical features where wider tolerances could reduce cost.

2. ASME Y14.5 Standards: Applied GD&T per ASME Y14.5 guidelines for all critical dimensions, with proper use of datums, feature control frames, and material condition modifiers.

Tolerance Analysis:

1. Worst-Case Stack-Up Analysis: Evaluated the cumulative effect of tolerances on critical assembly interfaces, ensuring proper function under worst-case manufacturing conditions.

2. Statistical Tolerance Analysis: Applied Root Sum of Squares (RSS) methodology for non-critical features to allow slightly wider individual tolerances while maintaining assembly capability, reducing manufacturing costs.

3. Geometric Tolerancing: Substituted geometric tolerances for plus/minus tolerances on key features (e.g., replacing linear dimensions with true position for hole patterns), providing clearer functional requirements and allowing more manufacturing flexibility.

Drawing Documentation:

1. Created comprehensive 2D manufacturing drawings with clear GD&T callouts for all precision components.

2. Documented surface finish requirements (Ra values) for bearing surfaces, sealing faces, and general surfaces.

3. Provided detailed inspection instructions for quality control during manufacturing.


Structural Analysis & Engineering Validation

Finite Element Analysis (FEA):

1. Load Analysis: Identified operational loads including self-weight (solar panel mounting, frame), dynamic loads (vibration from threshing drum), and static loads (hopper capacity, frame assembly).

2. Stress Validation: Simulated maximum von Mises stresses on the frame structure under worst-case loading conditions. Validated that stresses remained below the yield strength of the material with a safety factor of 2.0 (minimum).

3. Displacement Analysis: Evaluated maximum deflection of the frame under operational loads, confirming it remained within allowable limits to maintain rotor alignment.

4. Modal Analysis: Performed modal analysis to identify natural frequencies of key components, ensuring they didn't coincide with operational frequencies to prevent resonance.

Power Transmission Validation:

1. Motor Selection: Specified a 1.5kW brushless DC motor optimized for the design, paired with a 300W solar panel array and battery system based on energy balance calculations.

2. Belt Drive Analysis: Calculated center distances, belt tensions, and power transmission capacity to ensure efficient power transfer. Verified belt life using industry standards.

3. Bearing Selection: Determined bearing sizes (SKF 6203 and 6205 series) based on radial and thrust load calculations, with expected L10 life exceeding 20,000 hours.

Design Iteration & Optimization:
Based on analysis results, made the following design improvements:

1. Added gussets at high-stress weld joints to redistribute loads

2. Increased wall thickness in critical areas while reducing thickness in non-critical areas to maintain overall weight

3. Redesigned the solar mounting bracket to reduce leverage and improve frame stability


🔄 Reverse Engineering & Scan-to-CAD Capability

Application to This Project:
While this project was designed from scratch, I utilized reverse engineering methodologies during the development process:

1. Competitor Analysis: Performed scan-to-CAD conversion of three competitor machines to understand design approaches, identify best practices, and establish performance benchmarks.

2. Component Replication: Created CAD models of salvaged electric motors and bearings using caliper measurements and optical scanning, enabling the design of custom mounting interfaces.

3. Point Cloud Processing: Processed scans of existing machines to extract key design parameters (drum geometry, clearance dimensions, hopper angles), incorporating proven concepts while improving upon identified weaknesses.


📝 Design Documentation & Communication

Comprehensive Documentation Package:

Design Files:

1. Master assembly file with complete part file references

2. Individual part files with feature history and design intent notes

3. Drawing files with GD&T, dimensions, and tolerances

4. STEP and IGES neutral formats for supplier communication


Technical Documentation:

1. Engineering BOM (EBOM): Complete bill of materials with part numbers, quantities, materials, and sourcing specifications.

2. Manufacturing Instructions: Detailed fabrication guides for each manufacturing method (sheet metal cutting/bending schedules, CNC machining programs, injection molding specifications).

3. Assembly Instructions: Step-by-step assembly sequence with torque specifications for critical fasteners.

4. Quality Control Plan: Inspection points and acceptance criteria for incoming materials, in-process fabrication, and final assembly.

5. Operation Manual: User guide including setup, operation, maintenance, and troubleshooting instructions.

Change Management:

1. Documented all design iterations, recording version history with clear change descriptions.

2. Maintained revision control for all drawings and models.

3. Created traceability matrix linking design changes to analysis results and testing outcomes.

Collaboration & Communication:

1. Prepared technical reports for project stakeholders, clearly communicating design decisions, analysis results, and manufacturing considerations.

2. Created visual presentations with 3D renderings and exploded views for client demonstrations.

3. Drafted clear engineering briefs for suppliers, specifying requirements for sheet metal fabrication, CNC machining, and injection molding.


🛠️ Automation & Scripting (Python, iLogic, VBA)

Workflow Automation Applied to This Project:

Python Scripting:

1. Design Generation: Developed a Python script that generates new thresher configurations based on input parameters (crop type, desired throughput, solar panel size). The script adjusts key dimensions and recalculates power requirements automatically.

2. Data Extraction: Created a script to extract design parameters from the CAD model (weights, material volumes, center of gravity) for engineering analysis, reducing manual data entry.

3. BOM Generation: Automated BOM extraction and formatting for supplier communication.

VBA / iLogic Integration:

1. Automated Drawing Creation: Used iLogic within Inventor to automate drawing sheet creation, view placement, and dimensioning, reducing drafting time by 50%.

2. Design Rule Checks: Created iLogic rules to check for common design errors (e.g., wall thickness variations, sharp corners, missing draft angles) and flag them before manufacturing documentation.


📊 Project Outcomes & Impact

Measurable Results:

1. Labor Reduction: Reduces manual threshing labor by up to 70%—from 8 hours per 100kg to approximately 2.5 hours.

2. Grain Damage: Reduces grain breakage from ~15% (manual method) to ~3% (mechanical method), significantly improving marketable yield.

3. Fuel Savings: Eliminates diesel consumption entirely, saving farmers $150-$200 annually while reducing carbon emissions.

4. Throughput Capacity: Achieves processing capacity of 150-200kg per hour, suitable for smallholder farmers and cooperatives.

Manufacturing Feasibility:

1. Cost Target: Achieved a production cost target of $650-800 per unit, making the machine economically accessible to smallholder farmers.

2. Manufacturing Accessibility: Designed for local production using readily available materials and standard workshop equipment.

3. Maintainability: Service life of 5+ years with routine maintenance; designed with accessible service points and readily available replacement parts.


🔧 Skills Demonstrated in This Project

1. CAD Modeling: SolidWorks, Parametric Modeling, Assembly Modeling, Feature Tree Management.
   
2. Manufacturing: DFM, Injection Molding, Sheet Metal Design, CNC Machining, Casting, Forging.

3. Drafting & Tolerancing: GD&T (ASME Y14.5), Tolerance Application, Design Documentation.

4. Analysis: FEA, Structural Analysis, Load Analysis, Modal Analysis.
  
5. Automation: Python, iLogic, VBA, Design Tables, DriveWorks.
    
6. Engineering:	Reverse Engineering, Scan-to-CAD, Manufacturing Analysis.
    
7. Soft Skills:	Written Communication, Verbal Communication, Project Documentation, Problem Solving.


This project demonstrates that I can:

✅ Create complex parametric assemblies with robust feature trees and precise constraints

✅ Apply DFM principles across injection molding, sheet metal, CNC, and casting/forging

✅ Utilize GD&T per ASME Y14.5 with practical tolerance analysis

✅ Perform structural validation through FEA and mechanical analysis

✅ Automate design workflows using Python, iLogic, and VBA

✅ Generate comprehensive documentation for manufacturing and assembly

✅ Communicate design intent clearly through written reports and visual presentations

✅ Manage feature trees for maximum editability and stability

✅ Apply reverse engineering and scan-to-CAD methodologies where needed
























