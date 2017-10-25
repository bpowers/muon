use_relative_paths = True

deps = {
  "vendor/node": "https://github.com/brave/node.git@7535fd34c36a40403743af5bf71c5b79b3f0bb6d",
  "vendor/ad-block": "https://github.com/brave/ad-block.git@924110635eac11f824f92be111c0cb92cf559b30",
  "vendor/tracking-protection": "https://github.com/brave/tracking-protection.git@472bc47ef964a541e0ebe39dc63689e341471fdf",
  "vendor/hashset-cpp": "https://github.com/bbondy/hashset-cpp.git@8932637e565e70151dbe4bbb35990c6d41685763",
  "vendor/bloom-filter-cpp": "https://github.com/bbondy/bloom-filter-cpp.git@ba94da0192bf9b81a457ae27dea2602b9ee0facc",
  "vendor/requests": "https://github.com/kennethreitz/requests@e4d59bedfd3c7f4f254f4f5d036587bcd8152458",
  "vendor/boto": "https://github.com/boto/boto@f7574aa6cc2c819430c1f05e9a1a1a666ef8169b",
  "vendor/python-patch": "https://github.com/svn2github/python-patch@a336a458016ced89aba90dfc3f4c8222ae3b1403",
}

hooks = [
  {
    'name': 'bootstrap',
    'pattern': '.',
    'action': ['python', 'src/electron/script/bootstrap.py'],
  },
  {
    'name': 'update_external_binaries',
    'pattern': '.',
    'action': ['python', 'src/electron/script/update-external-binaries.py']
  },
  {
    # Apply patches to chromium src
    'name': 'apply_patches',
    'pattern': '.',
    'action': ['python', 'src/electron/script/apply-patches.py'],
  }
]
