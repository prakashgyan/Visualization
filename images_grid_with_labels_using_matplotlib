import matplotlib.image as mpimg
import matplotlib.pyplot as plt
from mpl_toolkits.axes_grid1 import ImageGrid

# list containing location of images to populate -- i have used some placeholders here- -
all_images_addr = ['https://via.placeholder.com/150', 'https://via.placeholder.com/150',
                   'https://via.placeholder.com/300', 'https://via.placeholder.com/300']
n_rows = 2
n_cols = 2

fig = plt.figure(figsize=(30., 30.), facecolor='white')
grid = ImageGrid(fig, 111, nrows_ncols=(n_rows, n_cols), axes_pad=.5)

for ax, img_addr in zip(grid, all_images_addr):
    img = mpimg.imread(img_addr)
    ax.imshow(img)
    ax.set_title(img_addr.split('/')[-1])  # custom title for the image extracted from location
    ax.set_axis_off()

plt.show()
