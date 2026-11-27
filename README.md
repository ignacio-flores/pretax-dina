# pretax-dina

This repository archives the code regional coordinators used to produce historical pretax national income series. In this first phase, give each region one self-contained folder for its code and run instructions. Keep the existing code layout wherever possible.

## Organize your contribution

- **Inputs.** Keep all inputs for your region in a single Dropbox folder and out of Git. Record the Dropbox location and the path inside the regional folder so another contributor can copy the entire input folder into their checkout in one step. Consolidate scattered inputs if needed.
- **Intermediate files.** Where practical, generate them locally and add them to `.gitignore`.
- **Outputs.** Where practical, write final tables, figures, and data to one folder so they can be exported together.
- **Credentials.** Keep passwords, API keys, and other secrets out of Git. If you store them in a document, save it locally in your region’s `confidential/` folder. Git ignores everything there except the `.gitkeep` placeholder.

## Example regional folder

```text
example-region/
├── README.md       # Run instructions
├── code/           # Scripts
├── inputs/         # Copied locally from Dropbox
├── intermediate/   # Generated locally
├── outputs/        # Final tables, figures, and data
└── confidential/   # Local credentials and a tracked .gitkeep placeholder
```

If you use this layout, update and uncomment the example `.gitignore` entries for your region’s `inputs/` and `intermediate/` folders.

## Verify before uploading

Run the code from a clean checkout with the Dropbox inputs and check that it reproduces the coordinator’s results for the same release. In your regional folder, record the input version, the software and dependencies needed, the command or script order, and the reference results you checked. Upload the code once the check passes.
