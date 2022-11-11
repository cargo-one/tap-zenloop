# tap-zenloop

This is a [Singer](https://singer.io) tap that produces JSON-formatted data
following the [Singer
spec](https://github.com/singer-io/getting-started/blob/master/SPEC.md).

This tap:

- Pulls raw data from the [Zenloop API](https://docs.zenloop.com/reference/introduction)
- Currently it only extracts answers to surveys, but this should be easy to extend for your own needs.
  - [Answers](https://docs.zenloop.com/reference/get-answers)
- Outputs the schema for each resource
- Incrementally pulls data based on the input state
