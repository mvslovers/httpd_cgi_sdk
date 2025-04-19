
# HTTPD CGI SDK

The **HTTPD CGI SDK** provides all the necessary header and source files to develop CGI (Common Gateway Interface) modules for Mike Rayborn's HTTPD server. This SDK streamlines the development process, allowing you to focus on building dynamic and powerful web applications.


## Getting Started

### Prerequisites

- Mike Rayborn's HTTPD server must be installed and running.
- A C compiler, such as GCCMVS, for building CGI modules.

### Installation

Clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/httpd-cgi-sdk.git
cd httpd-cgi-sdk
```

Include the SDK headers in your project or let your compiler use these `include` directory:

```bash
gccmvs -I{THIS_REPO_DIR}/inc -o my_cgi_module my_cgi_module.c
```

### Usage

1. Write your CGI module in C, including the necessary headers from the SDK.
2. Compile your code using a C compiler.
3. Deploy the compiled module to the CGI directory of the HTTPD server.

Example CGI module:

```c
#include "httpd.h"
#include "cgi.h"

int main() {
    printf("Content-Type: text/html\r\n\r\n");
    printf("<html><body><h1>Hello, world!</h1></body></html>");
    return 0;
}
```

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

Special thanks to **Mike Rayborn** for developing the HTTPD server and making this SDK possible.

---

Happy coding with HTTPD CGI SDK!

