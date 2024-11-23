# Define file names
dim_file = "DIM_List.txt"
diy_file = "DIY_List.txt"
auto_file = "Auto_List.txt"
trash_file = "Trash_List.txt"

# Read the contents of all files
with open(diy_file, "r") as diy:
    diy_list = diy.readlines()

with open(auto_file, "r") as auto:
    auto_list = auto.readlines()

with open(trash_file, "r") as trash:
    trash_list = trash.readlines()

with open(dim_file, "r") as dim:
    dim_list = dim.readlines()

# Combine DIY_List, Trash_List, and Auto_List in the specified order
combined_list = diy_list + trash_list + auto_list

# Merge the combined list into DIM_List starting at line 5
# Adjust line numbers since Python uses zero-based indexing
insert_position = 4  # Line 5 is index 4
updated_dim_list = dim_list[:insert_position] + combined_list + dim_list[insert_position:]

# Write the updated DIM_List back to the file
with open(dim_file, "w") as dim:
    dim.writelines(updated_dim_list)

print("DIM_List has been updated successfully!")
