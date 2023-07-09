# -email_updater_from_old_to_new
# Email Domain Replacement Program

This program processes a list of email addresses, replacing instances of the old domain with the new domain. The list of email addresses is read from a CSV file, and the updated list is written back to another CSV file.

## Functions

### `contains_domain(address, domain)`

Checks if the given email address contains the specified domain in the domain position.

- Parameters:
  - `address` (str): Email address to check.
  - `domain` (str): Domain to match.

- Returns:
  - `True` if the email address contains the specified domain in the domain position.
  - `False` if not.

### `replace_domain(address, old_domain, new_domain)`

Replaces the old domain with the new domain in the given email address.

- Parameters:
  - `address` (str): Email address to modify.
  - `old_domain` (str): Old domain to replace.
  - `new_domain` (str): New domain to use.

- Returns:
  - The modified email address with the old domain replaced by the new domain.

### `main()`

The main function of the program. It processes the list of emails, replacing instances of the old domain with the new domain.

- Reads the list of emails from a CSV file.
- Identifies the email addresses with the old domain and replaces them with the new domain.
- Writes the updated list of emails to a new CSV file.

## Usage

1. Ensure you have Python 3 installed.
2. Install the required dependencies, if any (e.g., `pip install csv`).
3. Prepare the CSV file containing the list of email addresses. Ensure it follows the required format.
4. Update the program's variables according to your needs:
   - `old_domain`: The old domain to replace.
   - `new_domain`: The new domain to use.
   - `csv_file_location`: The path to the input CSV file.
   - `report_file`: The path to the output CSV file.
5. Run the program: `python3 email_domain_replacement.py`.
6. Check the specified `report_file` for the updated list of email addresses.

## Example

```python
# Example usage of the program
old_domain = 'abc.edu'
new_domain = 'xyz.edu'
csv_file_location = '/path/to/input/file.csv'
report_file = '/path/to/output/updated_emails.csv'

# ... rest of the program ...
