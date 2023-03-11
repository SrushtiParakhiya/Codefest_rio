# Codefest_rio
def Township(T, N, totalbedroom, R, S, H):
    ans = []
    for i in range(T):
        asset_qty = 0
        normal_qty = 0
        total_hr = 0
        for j in range(N):
            totalWalls = N*6*H+N*4*S+N*3*R
            asset_walls = totalWalls/3
            normal_walls = (totalWalls*2)/3
            asset_qty += 1.5*asset_walls
            normal_qty += 2.25*normal_walls
            total_hr += (2.5*asset_walls+3.25*normal_walls)
            ans.append(asset_qty, normal_qty, total_hr)
    return ans
