# 🤝 Contributing Guidelines

Welcome to the **Genome-Sequencing** research repository! We are excited to collaborate on solving cutting-edge genomic problems using artificial intelligence. To maintain code quality, systematic documentation, and robust pipelines, please adhere to the following development standards.

---

## 🌿 Branching Strategy

We use a structured, developer-focused branching strategy. All work must be conducted on feature branches branched from `main`.

*   **Branch Naming Convention**: `name/task` (use lowercase and hyphens)
    *   *Examples*:
        *   `akshita/variant-pathogenicity-prediction`
        *   `abhiraj/assembly-graph-gnn`
        *   `samyak/eval-framework`
        *   `hitanshi/sc-rna-data-loader`
*   **Workflow**:
    1.  Pull the latest updates from `main`: `git pull origin main`
    2.  Create your branch: `git checkout -b name/task`
    3.  Commit your changes locally (see Commit Message Format below).
    4.  Push your branch to GitHub: `git push origin name/task`
    5.  Open a Pull Request (PR) targeting `main`. At least one team member must review and approve your PR before merging.

---

## 💬 Commit Message Format

We enforce **Conventional Commits** to keep our repository history clean and automatically parseable.

Format: `<type>(<scope>): <short summary>` (scope is optional)

### Common Types:
*   `feat`: A new feature (e.g., a new model architecture or data preprocessing script)
*   `fix`: A bug fix (e.g., fixing a tensor dimension mismatch in training)
*   `docs`: Documentation changes only (e.g., updating README or completing paper reviews)
*   `style`: Formatting, missing semi-colons, white-space changes (no code logic change)
*   `refactor`: Code changes that neither fix a bug nor add a feature, but improve code structure
*   `perf`: Code changes that improve performance (e.g., memory optimization or multi-GPU support)
*   `test`: Adding missing tests or correcting existing tests
*   `chore`: Internal maintenance tasks (e.g., updating dependencies or package manager setup)

### Examples:
*   `feat(models): implement Enformer sequence encoder for multi-scale expression`
*   `fix(utils): resolve out-of-memory bug in BAM file chunk reader`
*   `docs(reviews): complete literature review for AlphaMissense paper`
*   `chore(deps): upgrade torch to 2.1.0 and flash-attention`

---

## 📚 Literature Review Submission Rules

To ensure high scientific quality and consistency, all literature review entries must fulfill these criteria:

1.  **Strict Template Compliance**: Every review must follow the structural format pre-allocated in your dedicated review files.
2.  **Coverage**: All members must review the **4 shared papers** and their **5 self-selected papers** (total of 9 reviews).
3.  **Completeness**: No review section should be left blank or filled with placeholder text. Each section (Problem, Methodology, Key Results, Limitations, Future Scope, and Relevance) must be filled with robust, expert-level analysis (not generic copy-paste).
4.  **Submission Path**: Navigate to your pre-created folder under `literature-review/members/<your-folder-name>/` and fill out your answers inside the individual files `paper-1.md` through `paper-9.md`. Do not commit files outside your designated folder.

---

## 🚫 Data Management Rules (Strict)

Genomic datasets (FASTQ, FASTA, BAM, VCF, etc.) are extremely large and **MUST NOT** be committed to the Git repository.

*   **No Raw Data in Repo**: Any attempt to push raw datasets, sample files, database dumps, or model weights will be rejected.
*   **Gitignore Compliance**: Ensure that all data directories and binary outputs are captured under `.gitignore`.
*   **External Storage**: Store large datasets in our shared external storage (e.g., Google Cloud Storage, AWS S3, or reference databases like NCBI, gnomAD) and use lightweight downloading/loading scripts (`datasets/download_scripts.py`) to fetch data locally when running pipelines.
*   **Sample Data**: If mock or dummy data is necessary for unit testing, keep the files under 50KB and place them strictly in a `tests/test_data/` directory.

---

## 🛠️ Pull Request & Review Process

Before merging any code or documentation into `main`:
1.  Verify that your code complies with standard Python PEP8 formatting (use `black` and `flake8`).
2.  Ensure that all tests pass: `pytest`
3.  Open a Pull Request with a clear explanation of what was changed and why it was changed.
4.  Request a review from at least one peer or the Team Lead. Address any feedback before merging.

Thank you for helping us maintain a world-class research environment! Let's build something extraordinary. 🚀
