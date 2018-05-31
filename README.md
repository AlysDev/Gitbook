# Gitbook
Premier exercice

import React from "react";
import { render } from "react-dom";
import EXAMPLE_DOCUMENT from "./EXAMPLE_DOCUMENT.json";

class DocumentRenderer extends React.Component {
  render() {
    // The document to render is provided as a prop
    const document = this.props.document;

    return (
      <div>
        <p>
          The first exercise will ask you to render a document here. <br />
          You can edit the files, and the code in <code>index.js</code>, and the
          right pane will update automatically {"\u2728"}.
        </p>
      </div>
    );
  }
}

render(
  <DocumentRenderer document={EXAMPLE_DOCUMENT} />,
  document.getElementById("root")
);
