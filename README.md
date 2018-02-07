# com.niktaxi.membershipperiods

This extension adds Membership Periods: with every membership renewal or edit, separate membership periods are stored. They can be viewed on membership's details page. Additionally, membership's periods have links to contribution that renewed it.

This extension is created as a test for Compucorp application process and is not ready for production deployment

![Screenshot](/images/screenshot.png) 


The extension is licensed under [AGPL-3.0](LICENSE.txt).

## Requirements

* PHP v7.0+
* CiviCRM 4.7+

## Usage

This extension does not require any changes in how the memberships are edited/renewed - membership periods will be stored automatically. Initially, every membership will have only one period (created during extension's installation) with dates copied from entire membership duration.

Membership periods are visible on a membership's details form for every contact. There's also a link for a contribution, if it was done during renewal.

## Known Issues

- shortening membership (moving membership end date back or membership start date forward) removes link between contribution and changed membership period
