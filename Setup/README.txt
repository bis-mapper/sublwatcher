
    Product Title (PRODUCT)
    Version xx.xxx
    _______________________________________________________________


    General Description
    -------------------
    Product description goes here ...




    Server Requirements
    -------------------
    PRODUCT runs on all current BIS platforms, including Windows,
    Linux/Unix and ClearPath/2200.


    Client Workstation Requirements
    -------------------------------
    A GUI workstation (GI/MPC) is required to install and execute
    PRODUCT.


    Database Requirements
    ---------------------
    - One empty BIS database drawer
    - Approximately nnn MB of BIS database space

    _______________________________________________________________


    Installation
    ------------
    The PRODUCT Setup Wizard guides you through the installation
    process, and automatically loads and registers all required
    programs and tables.


    Note:
    -----
    If you downloaded a ZIP file containing the PRODUCT package,
    you must first unZIP it to an empty directory.  Then follow
    the steps below, and specify that directory path when prompted.


    Follow these steps to load the PRODUCT software:

    1. Sign on to the BIS system with coordination privileges
       (i.e., MAPCOORD user-id).  For ClearPath/2200 systems,
       your user-id must also have permission to execute the
       GEN function.

    2. Execute PCMA, and select Load/Setup Application Package.
       (Or use fast access call to bypass PCMA: PCME,SETUP)
       IF PCMA is not available, execute the SETUP utility.
       If you cannot access either PCMA or SETUP, use the
       Alternate Installation Method below.

    3. Specify the location of the PRODUCT installation software
       (CD-ROM or hard drive path containing the PRODUCT package)
       and follow the simple step-by-step Wizard instructions.


    Alternate Installation Method
    -----------------------------
    1. Upload (using the PCX utility) the SETUP.RUN file from the
       CD-ROM or hard drive path containing the PRODUCTsoftware.

    2. Register the uploaded report as a run script with:
       - 99999 I/Os and LLPs
       - Access to ALL cabinets.

    3. Execute this run script and follow the Wizard instructions.

