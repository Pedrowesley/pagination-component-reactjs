
# Pagination Component - ReactJS

Welcome to the Pagination Component repository!

## Description

The Pagination Component is a React component designed to simplify pagination for API requests. It provides easy navigation through paginated responses from API endpoints.

## Usage

To use the GitHub Pagination Component in your React project, follow these steps:

1. Clone the GitHub repository:

    ```bash
    git clone https://github.com/Pedrowesley/pagination-component-reactjs.git
    ```

2. Copy the `Pagination.js` file into your project.

3. Import the `Pagination` component into your React code:

    ```javascript
    import { Pagination } from './Pagination';
    ```

4. Use the `Pagination` component in your code, providing the necessary props:

    ```javascript
    <Pagination totalItems={totalItems} pagesAmount={pagesAmount} selectPage={selectPage} />
    ```

## Features

- **Efficient Pagination:** Divide large datasets into manageable pages for easier navigation.
- **Customizable:** Adjust the number of pages displayed per pagination instance.
- **Simple Integration:** Easily integrate into your React projects by copying the component file.

## Component Structure

The `Pagination` component is structured as follows:

- **totalItems:** Total number of items to paginate.
- **pagesAmount:** Number of pages to display at once.
- **selectPage:** Function to handle page selection.

## Example

Here's an example of how you can use the `Pagination` component in your React project:

```javascript
import React, { useState } from 'react';
import { Pagination } from './Pagination';

function App() {
  const [currentPage, setCurrentPage] = useState(1);
  const totalPages = 10; // Example total number of pages

  const handlePageChange = (pageNumber) => {
    setCurrentPage(pageNumber);
    // Fetch data for the new page from GitHub API
  };

  return (
    <div className="App">
      <h1>GitHub Pagination Example</h1>
      <Pagination
        totalItems={totalPages}
        pagesAmount={3}
        selectPage={handlePageChange}
      />
    </div>
  );
}

export default App;
```

## Contributing

Contributions to the GitHub Pagination Component are welcome! Feel free to open issues or submit pull requests for any improvements or bug fixes.

## License

This project is licensed under the [MIT License](LICENSE).

---

Feel free to customize this README further to include any additional information or details specific to your component.
