# OpenTaxSolver

- [Homepage](http://opentaxsolver.sourceforge.net/)

**OpenTaxSolver** (OTS) is a set of programs and templates for helping
you fill out your income tax forms. It performs the tedious arithmatic.

OTS is intented to assist those who normally prepare their tax forms
themselves, and who generally know on which lines to enter their
numbers. It is meant to be used in combination with the instruction
booklet corresponding to a given form.

## Usage

Example tax-data files and blank starting templates are included under
the `tax_form_files/` directory. For each filer, save a filled-out
template to a new name, such as `fed1040_2020.txt`. After filling in
the lines, run the tax solver on it. From the GUI, this is done by
pressing "Compute Tax" button.

Or solvers can be run from the command line, for example, as:

```
./bin/taxsolve_usfed1040_2020 fed1040_2020.txt
```

Where `fed1040_2020.txt` is the name of *uour* tax-data file, which you
edit with any text editor to fill it in or print it out. Output results
are saved to `..._out.txt` files (e.g., `fed1040_2020_out.txt`), and
can be printed out directly too.

### Automatic PDF form fill-out

OTS also contains an automatic PDF form fill-out function.

- Supports all federal forms and state forms
- Saves time by filling out many of the numbers
- You may still need to enter some information or check boxes that are
  not handled by OTS
- Tested to work properly with many viewers

For automatic fill-out of PDF forms, click the "Print" button and
select "Automatically Fill-out PDF Tax-Form", then click "Print".

You can set your preferred PDF viewer by the "Set PDF Viewer" button,
or by setting the environment variable `PDF_VIEWER`.

The automatic fill-out feature is tested to work properly with the
following PDF viewers:

- "Atril"
- "Firefox"
- "Google-Chrome"
- "IE"
- "LibreOffice"
- "Safari"
- "Xpdf"

## Legal

This program is made available under the terms of the GNU General
Public License, version 2.0 or later. See
[LICENSE](./LICENSES/GPL-2.0.txt) for details.

- [Contributors](http://opentaxsolver.sourceforge.net/credits.html)
