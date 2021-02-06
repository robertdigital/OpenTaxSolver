# Changelog

## v16.07 (2019-04-01)

* Added PDF metadata for California Schedule CA (540) 2018, Part II,
  Line 4, column A.
* On US 1040, adjusted calling of `SocSec_Worksheet()` until after
  Schedule-1 line 32, on which it could depend.

## v16.06 (2019-03-28)

* Fixed new GUI-bug that was introduced in last update, which could
  cause some line semi-colons, for newly added line-values, to be
  misplaced in save-files.

## v16.05 (2019-03-21)

* Improved GUI display formatting, and save-file formatting.
* Fixed NJ-State lines 74 + 75, and PDF positioning of line 17.
* Fixed GUI issue when loading State template(s) which did not display
  spouse fields when importing joint Federal return.

## v16.04 (2019-03-15)

* Added optional AMT worksheet line inputs to the Fed 1040 template.
* The AMT worksheet lines 2a through 2g now display in the PDF outputs.
* The OTS GUI now catches forced kills by the window manager when user
  clicks the "X" in the window tab, which now eliminates hanging zombie
  processes under MS-Windows.
* The "MarkupPDF" construct now supports quoted string values. This
  enables proper PDF display of multi-word answers, as well as
  explicit/literal character sequences without numeric formating.

## v16.03 (2019-03-08)

- Added Sched-B Part-III lines to the US-1040 (ticket #63).
* Added PDF metadata for dependent and occupation fill-in tags, so
  users can add these to their results output file (`_out.txt`) to
  fill-out the PDF forms (ticket #64).
* Added ability to add additional PDF mark-ups, or change them, from
  your Tax Input Files, by adding "MarkupPDF" lines -- documented under
  OTS's "Data Input Format" web page.
* Added ability to comment-out lines of your result files (`_out.txt`)
  by placing exclamation mark "!" as first character on a line.
* Commented lines will be ignored by the PDF generator (ticket #65).
* Fixed NY State importing of Fed Sched-1 data (ticket #66), and
  warning on line 17 (ticket #67).

## v16.02 (2019-02-28)

* To the Federal form, added Alimony recipient info, which is then also
  imported by some state forms.
* Fixed some PDF positioning on federal form, including fields on the
  AMT form's second page.
* Added option to print all federal forms, even when not required, the
  `-allforms` option.
* From California template, removed CA540 line 5 which is imported from
  federal form, and broke out line 21 a-f.
* Fixed CA540 handling of SocSec payments, and CA540 line 10.

## v16.01 (2019-02-27)

* A fix to Fed 1040 line 55, as well as fixes for NJ and CA state
  programs.
* Added Health-Coverage field to federal template.
* Improved and added more active fields on several PDF forms.
* No longer requires spouse inputs when not filing jointly.
* Added alimony recipient fields for those who need it.

## v16.00 (2019-02-02)

* Initial Release for Tax-Year 2018.
